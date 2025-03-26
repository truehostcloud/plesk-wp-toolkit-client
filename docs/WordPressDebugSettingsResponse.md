# WordPressDebugSettingsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**wp_debug** | **bool** | WP_DEBUG setting | 
**wp_debug_log** | **bool** | WP_DEBUG_LOG setting | 
**wp_debug_display** | **bool** | WP_DEBUG_DISPLAY setting | 
**script_debug** | **bool** | SCRIPT_DEBUG setting | 
**save_queries** | **bool** | SAVEQUERIES setting | 

## Example

```python
from plesk_wp_toolkit_client.models.word_press_debug_settings_response import WordPressDebugSettingsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of WordPressDebugSettingsResponse from a JSON string
word_press_debug_settings_response_instance = WordPressDebugSettingsResponse.from_json(json)
# print the JSON string representation of the object
print(WordPressDebugSettingsResponse.to_json())

# convert the object into a dict
word_press_debug_settings_response_dict = word_press_debug_settings_response_instance.to_dict()
# create an instance of WordPressDebugSettingsResponse from a dict
word_press_debug_settings_response_from_dict = WordPressDebugSettingsResponse.from_dict(word_press_debug_settings_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


