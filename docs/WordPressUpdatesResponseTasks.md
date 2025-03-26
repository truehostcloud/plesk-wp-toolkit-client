# WordPressUpdatesResponseTasks


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**update** | [**BackgroundTaskResponse**](BackgroundTaskResponse.md) |  | 
**check** | [**BackgroundTaskResponse**](BackgroundTaskResponse.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.word_press_updates_response_tasks import WordPressUpdatesResponseTasks

# TODO update the JSON string below
json = "{}"
# create an instance of WordPressUpdatesResponseTasks from a JSON string
word_press_updates_response_tasks_instance = WordPressUpdatesResponseTasks.from_json(json)
# print the JSON string representation of the object
print(WordPressUpdatesResponseTasks.to_json())

# convert the object into a dict
word_press_updates_response_tasks_dict = word_press_updates_response_tasks_instance.to_dict()
# create an instance of WordPressUpdatesResponseTasks from a dict
word_press_updates_response_tasks_from_dict = WordPressUpdatesResponseTasks.from_dict(word_press_updates_response_tasks_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


