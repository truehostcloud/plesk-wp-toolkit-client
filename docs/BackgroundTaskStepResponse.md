# BackgroundTaskStepResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** | Code | 
**title** | **str** | Title | 
**icon** | **str** | Icon | 
**progress** | **float** | Progress | 
**status** | **str** | Status | 
**hint** | **str** | Hint | 

## Example

```python
from plesk_wp_toolkit_client.models.background_task_step_response import BackgroundTaskStepResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundTaskStepResponse from a JSON string
background_task_step_response_instance = BackgroundTaskStepResponse.from_json(json)
# print the JSON string representation of the object
print(BackgroundTaskStepResponse.to_json())

# convert the object into a dict
background_task_step_response_dict = background_task_step_response_instance.to_dict()
# create an instance of BackgroundTaskStepResponse from a dict
background_task_step_response_from_dict = BackgroundTaskStepResponse.from_dict(background_task_step_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


