# WordPressDebugStatusResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **bool** | Status | 

## Example

```python
from plesk_wp_toolkit_client.models.word_press_debug_status_response import WordPressDebugStatusResponse

# TODO update the JSON string below
json = "{}"
# create an instance of WordPressDebugStatusResponse from a JSON string
word_press_debug_status_response_instance = WordPressDebugStatusResponse.from_json(json)
# print the JSON string representation of the object
print(WordPressDebugStatusResponse.to_json())

# convert the object into a dict
word_press_debug_status_response_dict = word_press_debug_status_response_instance.to_dict()
# create an instance of WordPressDebugStatusResponse from a dict
word_press_debug_status_response_from_dict = WordPressDebugStatusResponse.from_dict(word_press_debug_status_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


