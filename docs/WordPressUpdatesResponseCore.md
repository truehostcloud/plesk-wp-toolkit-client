# WordPressUpdatesResponseCore


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**version** | **str** |  | 
**available_version** | **str** |  | 
**restore_point** | [**InstallationRestorePoint**](InstallationRestorePoint.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.word_press_updates_response_core import WordPressUpdatesResponseCore

# TODO update the JSON string below
json = "{}"
# create an instance of WordPressUpdatesResponseCore from a JSON string
word_press_updates_response_core_instance = WordPressUpdatesResponseCore.from_json(json)
# print the JSON string representation of the object
print(WordPressUpdatesResponseCore.to_json())

# convert the object into a dict
word_press_updates_response_core_dict = word_press_updates_response_core_instance.to_dict()
# create an instance of WordPressUpdatesResponseCore from a dict
word_press_updates_response_core_from_dict = WordPressUpdatesResponseCore.from_dict(word_press_updates_response_core_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


