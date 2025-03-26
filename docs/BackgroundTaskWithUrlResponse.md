# BackgroundTaskWithUrlResponse

Created

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **str** | Background task URL | 
**task** | [**BackgroundTaskResponse**](BackgroundTaskResponse.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.background_task_with_url_response import BackgroundTaskWithUrlResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BackgroundTaskWithUrlResponse from a JSON string
background_task_with_url_response_instance = BackgroundTaskWithUrlResponse.from_json(json)
# print the JSON string representation of the object
print(BackgroundTaskWithUrlResponse.to_json())

# convert the object into a dict
background_task_with_url_response_dict = background_task_with_url_response_instance.to_dict()
# create an instance of BackgroundTaskWithUrlResponse from a dict
background_task_with_url_response_from_dict = BackgroundTaskWithUrlResponse.from_dict(background_task_with_url_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


