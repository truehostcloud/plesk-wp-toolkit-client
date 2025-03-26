# BackgroundTaskResponse


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
from plesk_wp_toolkit_client.models.background_task_response import BackgroundTaskResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundTaskResponse from a JSON string
background_task_response_instance = BackgroundTaskResponse.from_json(json)
# print the JSON string representation of the object
print(BackgroundTaskResponse.to_json())

# convert the object into a dict
background_task_response_dict = background_task_response_instance.to_dict()
# create an instance of BackgroundTaskResponse from a dict
background_task_response_from_dict = BackgroundTaskResponse.from_dict(background_task_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


