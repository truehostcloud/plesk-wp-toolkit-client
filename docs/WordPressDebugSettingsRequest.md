# WordPressDebugSettingsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**wp_debug** | **bool** | WP_DEBUG setting | [optional] 
**wp_debug_log** | **bool** | WP_DEBUG_LOG setting | [optional] 
**wp_debug_display** | **bool** | WP_DEBUG_DISPLAY setting | [optional] 
**script_debug** | **bool** | SCRIPT_DEBUG setting | [optional] 
**save_queries** | **bool** | SAVEQUERIES setting | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.word_press_debug_settings_request import WordPressDebugSettingsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of WordPressDebugSettingsRequest from a JSON string
word_press_debug_settings_request_instance = WordPressDebugSettingsRequest.from_json(json)
# print the JSON string representation of the object
print(WordPressDebugSettingsRequest.to_json())

# convert the object into a dict
word_press_debug_settings_request_dict = word_press_debug_settings_request_instance.to_dict()
# create an instance of WordPressDebugSettingsRequest from a dict
word_press_debug_settings_request_from_dict = WordPressDebugSettingsRequest.from_dict(word_press_debug_settings_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


