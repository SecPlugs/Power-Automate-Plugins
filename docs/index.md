---
layout: none
---
Power Automate connectors to send docs, emails and attachments for analysis in your work flows.  
GDrive and GMail, Drop Box, and Exchange templates also provided.


## Usage
You use this {brand-plugin} within the context of Microsoft Power Automate platform

### Scan A File

#### Parameters
Use the following parameters to scan an email

|Name|Key|Required|Type|Description|
|--- |--- |--- |--- |--- |
|API Key|x-api-key||string| API Key|
|Client Id|x-client-id||string|Client Id to distinguish user|
|File Name|filename|True|string|File name of email|
|File Data ( Base64 encoded)|data|True|string|Base64 encoded File contents|

#### Returns
The following is returned 

|Name|Path|Type|Description|
|--- |--- |--- |--- |
|score|score|integer|score|
|sha256|threat_object.sha256|string|sha256 of file content|
|file_name|scan_context.file_name|string|scanned file name|
|client_id|scan_context.client_id|string|client Id of caller.|
|datetime|datetime|float|Time of scan|
|status|status|string|status of scan|
|account_id|account_id|string|account id of the user scanned|
|api_key|api_key|string|api key of caller|
|type|meta_data.plugin_info.type|string|type of the plugin calling secplugs|
|name|meta_data.plugin_info.name|string|name of the plugin|
|capability|meta_data.capability|string|capability of scan|
|vendor_config_name|meta_data.vendor_info.vendor_config_name|string|vendor configuration name|
|entitlement_level|meta_data.vendor_info.entitlement_level|string|entitlement level of file|
|vendor|meta_data.vendor_info.vendor|string|vendor name|
|credits|meta_data.vendor_info.credits|integer|credits of the user|
|report_id|report_id|string|report id of result|
|verdict|verdict|string|verdict of scan|
|duration|duration|float|duration taken in scan|
|user_report_url|user_report_url|string|user report url can be opened from browser.|


### Scan Email

#### Parameters

Use the following parameters to scan an email

#### Returns

The following is returned 

|Name|Path|Type|Description|
|--- |--- |--- |--- |
|score|score|integer|score of email scanned|
|email_id|threat_object.email_id|string|email id of email sender.|
|file_name|scan_context.file_name|string|email file name|
|client_id|scan_context.client_id|string|client id of caller|
|datetime|datetime|float|datetime of scan|
|status|status|string|status fo scan|
|account_id|account_id|string|account id of user|
|api_key|api_key|string|api key of user|
|type|meta_data.plugin_info.type|string|type of plugin|
|name|meta_data.plugin_info.name|string|name of plugin|
|capability|meta_data.capability|string|capability of email scan|
|vendor_config_name|meta_data.vendor_info.vendor_config_name|string|vendor configuration name|
|entitlement_level|meta_data.vendor_info.entitlement_level|string|entitlement level of email|
|vendor|meta_data.vendor_info.vendor|string|vendor of the email scan|
|credits|meta_data.vendor_info.credits|integer|credits left for user account|
|report_id|report_id|string|reportid of email scan result|
|verdict|verdict|string|verdict of email scan|
|duration|duration|float|time taken in email scan|
|user_report_url|user_report_url|string|user report url of email scan|


## Contact
Having trouble? [Contact {brand-name} ](https://{brand-root-domain}/contacts)