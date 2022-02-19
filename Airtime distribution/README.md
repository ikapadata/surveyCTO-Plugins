# Airtime & Data Distribution

## Description

This field plug-in is designed to recharge mobile devices with airtime and data worldwide. With it's [Relodaly](https://reloadly.com) API integration you have borderless recharges of 5 billion devices covered by 630 mobile operator networks in over 150 countries

### Features

1. Perform airtime reacharges to approximately 5 billion devices worldwide.
1. Perform data bundle recharges to approximately 5 billion devices worldwide.

### Data format

This field plug-in requires the `text` field type..

## How to use

### Getting started

**To use this plug-in as-is**

1. Download the [sample form]() from this repo and upload it to your SurveyCTO server.
1. Download the [recharges.fieldplugin.zip]() file from this repo, and attach it to the sample form on your SurveyCTO server.

### Parameters
#### Reloadly Recharges

| Parameter key | Parameter value |
| --- | --- |
| `phone` | international mobile phone number|
| `network` | moblie network operator name|
| `amount` | value of recharge|
| `category` | specify Airtime or Data recharge|
| `reloadlyId` | reloadly API ID|
| `reloadlySecret` | Reloadly Secret API Key|


### Example
To display a percent symbol on the right of the textbox, the following would be placed in the appearance column of the spreadsheet form definition:

`custom-format-symbol(symbol='%', placement='right')`

### Default SurveyCTO feature support

| Feature / Property | Support |
| --- | --- |
| Supported field type(s) | `decimal`|
| Default values | Yes |
| Constraint message | Uses default behavior |
| Required message | Uses default behavior |
| media:image | Yes |
| media:audio | Yes |
| media:video | Yes |
| `show-formatted` appearance | No |

## More resources

* **Sample form**   
[Download sample form](https://github.com/surveycto/format-symbol/raw/master/extras/sample-form/Sample%20form%20-%20Format%20symbol%20field%20plug-in.xlsx)  

* **Developer documentation**  
Instructions and resources for developing your own field plug-ins.  
[https://github.com/surveycto/Field-plug-in-resources](https://github.com/surveycto/Field-plug-in-resources)

* **User documentation**  
How to get started using field plug-ins in your SurveyCTO form.  
[https://docs.surveycto.com/02-designing-forms/03-advanced-topics/06.using-field-plug-ins.html](https://docs.surveycto.com/02-designing-forms/03-advanced-topics/06.using-field-plug-ins.html)
