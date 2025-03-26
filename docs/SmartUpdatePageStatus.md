# SmartUpdatePageStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**http_status** | **int** | HTTP status | 
**page_title** | **str** | Page title | 
**response_incorrectness** | **bool** | HTTP response code changed | 
**page_fetching_error_code** | **int** | Error code | [optional] 
**php_errors** | **List[str]** | PHP errors | 
**php_notices** | **List[str]** | PHP notices | 
**php_warnings** | **List[str]** | PHP warnings | 
**shortcodes** | **List[str]** | Broken shortcodes | 

## Example

```python
from plesk_wp_toolkit_client.models.smart_update_page_status import SmartUpdatePageStatus

# TODO update the JSON string below
json = "{}"
# create an instance of SmartUpdatePageStatus from a JSON string
smart_update_page_status_instance = SmartUpdatePageStatus.from_json(json)
# print the JSON string representation of the object
print(SmartUpdatePageStatus.to_json())

# convert the object into a dict
smart_update_page_status_dict = smart_update_page_status_instance.to_dict()
# create an instance of SmartUpdatePageStatus from a dict
smart_update_page_status_from_dict = SmartUpdatePageStatus.from_dict(smart_update_page_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


