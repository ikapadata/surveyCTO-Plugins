# Airtime & Data Distribution

## Description

This field plug-in is designed to recharge mobile devices with airtime and data worldwide. With it's [Relodaly](https://reloadly.com) API integration you have borderless recharges of 5 billion devices covered by 630 mobile operator networks in over 150 countries

### Features

1. Perform airtime reacharges to approximately 5 billion devices worldwide.
1. Perform data bundle recharges to approximately 5 billion devices worldwide.

### Data format

This field plug-in is used in the `text` field type.

## How to use

### Getting started

**To use this plug-in as-is**

1. Download the [sample form]() from this repo and upload it to your SurveyCTO server.
1. Download the [recharges.fieldplugin.zip]() file from this repo, and attach it to the sample form on your SurveyCTO server.

### Parameters
#### Reloadly Recharges
[Create a Reloadly account] and find your `reloadlyId` and `reloadlySecret` at [API settings.](https://www.reloadly.com/developers/api-settings)
| Parameter key | Parameter value |
| --- | --- |
| `phone` | recipient's international mobile phone number|
| `network` | moblie network operator name|
| `amount` | value of recharge|
| `isoNmae` | Country ISO name of the receipient|
| `category` | specify Airtime or Data recharge|
| `reloadlyId` | reloadly API ID|
| `reloadlySecret` | Reloadly Secret API Key|


### Example
To recharge a South African phone number with airtime worth 100 ZAR:

```custom-recharges(phone='27801234567',amount='100', network='Vodacom - South Africa', isonName='ZA', reloadlyId='INSERT_RELOADLY_ID', reloadlySecret='INSERT_RELOADLY_SECRET_KEY',category='Airtime')```

To recharge a South African phone number with data worth 100MB:

`custom-recharges(phone='27801234567',amount='100MB', network='Vodacom - South Africa', isonName='ZA', reloadlyId='INSERT_RELOADLY_ID', reloadlySecret='INSERT_RELOADLY_SECRET_KEY',category='Data')`

## More resources

* **Sample form**   
[Download sample form]()  

* **Developer documentation**  
Instructions and resources for developing your own field plug-ins.  
[https://github.com/surveycto/Field-plug-in-resources](https://github.com/surveycto/Field-plug-in-resources)

* **User documentation**  
How to get started using field plug-ins in your SurveyCTO form.  
[https://docs.surveycto.com/02-designing-forms/03-advanced-topics/06.using-field-plug-ins.html](https://docs.surveycto.com/02-designing-forms/03-advanced-topics/06.using-field-plug-ins.html)
