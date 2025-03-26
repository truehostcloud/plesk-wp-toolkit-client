# IntegrityTasks


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reinstall** | [**BackgroundTaskResponse**](BackgroundTaskResponse.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.integrity_tasks import IntegrityTasks

# TODO update the JSON string below
json = "{}"
# create an instance of IntegrityTasks from a JSON string
integrity_tasks_instance = IntegrityTasks.from_json(json)
# print the JSON string representation of the object
print(IntegrityTasks.to_json())

# convert the object into a dict
integrity_tasks_dict = integrity_tasks_instance.to_dict()
# create an instance of IntegrityTasks from a dict
integrity_tasks_from_dict = IntegrityTasks.from_dict(integrity_tasks_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


