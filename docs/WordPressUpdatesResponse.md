# WordPressUpdatesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **float** |  | 
**applicable** | **bool** |  | 
**display_title** | **str** |  | 
**title** | **str** |  | 
**multisite** | **bool** |  | 
**vulnerable** | **bool** |  | 
**last_check_update_timestamp** | **int** |  | 
**smart_update** | [**WordPressUpdatesSmartUpdatesResponse**](WordPressUpdatesSmartUpdatesResponse.md) |  | 
**core** | [**WordPressUpdatesResponseCore**](WordPressUpdatesResponseCore.md) |  | 
**plugins** | [**List[InstallationPlugin]**](InstallationPlugin.md) |  | 
**themes** | [**List[InstallationTheme]**](InstallationTheme.md) |  | 
**auto_update** | [**InstallationAutoUpdateResponse**](InstallationAutoUpdateResponse.md) |  | 
**tasks** | [**WordPressUpdatesResponseTasks**](WordPressUpdatesResponseTasks.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.word_press_updates_response import WordPressUpdatesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of WordPressUpdatesResponse from a JSON string
word_press_updates_response_instance = WordPressUpdatesResponse.from_json(json)
# print the JSON string representation of the object
print(WordPressUpdatesResponse.to_json())

# convert the object into a dict
word_press_updates_response_dict = word_press_updates_response_instance.to_dict()
# create an instance of WordPressUpdatesResponse from a dict
word_press_updates_response_from_dict = WordPressUpdatesResponse.from_dict(word_press_updates_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


