# SmartPhpUpdateStubResponseMetaTasksUpdate

Smart PHP Update task

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | ID | 
**code** | **str** | Code | 
**title** | **str** | Title | 
**status** | **str** | Status | 
**progress** | **float** | Progress | 
**steps** | [**List[BackgroundTaskStepResponse]**](BackgroundTaskStepResponse.md) | Steps | 
**public_params** | **object** | Public parameters | 
**errors** | **List[str]** | Errors | 

## Example

```python
from plesk_wp_toolkit_client.models.smart_php_update_stub_response_meta_tasks_update import SmartPhpUpdateStubResponseMetaTasksUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of SmartPhpUpdateStubResponseMetaTasksUpdate from a JSON string
smart_php_update_stub_response_meta_tasks_update_instance = SmartPhpUpdateStubResponseMetaTasksUpdate.from_json(json)
# print the JSON string representation of the object
print(SmartPhpUpdateStubResponseMetaTasksUpdate.to_json())

# convert the object into a dict
smart_php_update_stub_response_meta_tasks_update_dict = smart_php_update_stub_response_meta_tasks_update_instance.to_dict()
# create an instance of SmartPhpUpdateStubResponseMetaTasksUpdate from a dict
smart_php_update_stub_response_meta_tasks_update_from_dict = SmartPhpUpdateStubResponseMetaTasksUpdate.from_dict(smart_php_update_stub_response_meta_tasks_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


