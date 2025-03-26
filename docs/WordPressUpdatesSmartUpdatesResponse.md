# WordPressUpdatesSmartUpdatesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **bool** | Smart Update enabled | 
**task_status** | [**InstallationSmartUpdatesTaskStatusEnum**](InstallationSmartUpdatesTaskStatusEnum.md) |  | 
**applicable** | **bool** |  | 

## Example

```python
from plesk_wp_toolkit_client.models.word_press_updates_smart_updates_response import WordPressUpdatesSmartUpdatesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of WordPressUpdatesSmartUpdatesResponse from a JSON string
word_press_updates_smart_updates_response_instance = WordPressUpdatesSmartUpdatesResponse.from_json(json)
# print the JSON string representation of the object
print(WordPressUpdatesSmartUpdatesResponse.to_json())

# convert the object into a dict
word_press_updates_smart_updates_response_dict = word_press_updates_smart_updates_response_instance.to_dict()
# create an instance of WordPressUpdatesSmartUpdatesResponse from a dict
word_press_updates_smart_updates_response_from_dict = WordPressUpdatesSmartUpdatesResponse.from_dict(word_press_updates_smart_updates_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


