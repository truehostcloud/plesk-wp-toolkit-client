# WordPressDebugStatusRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **bool** | Status | 

## Example

```python
from plesk_wp_toolkit_client.models.word_press_debug_status_request import WordPressDebugStatusRequest

# TODO update the JSON string below
json = "{}"
# create an instance of WordPressDebugStatusRequest from a JSON string
word_press_debug_status_request_instance = WordPressDebugStatusRequest.from_json(json)
# print the JSON string representation of the object
print(WordPressDebugStatusRequest.to_json())

# convert the object into a dict
word_press_debug_status_request_dict = word_press_debug_status_request_instance.to_dict()
# create an instance of WordPressDebugStatusRequest from a dict
word_press_debug_status_request_from_dict = WordPressDebugStatusRequest.from_dict(word_press_debug_status_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


