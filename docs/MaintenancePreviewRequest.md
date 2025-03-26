# MaintenancePreviewRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**texts** | [**MaintenanceTextsRequest**](MaintenanceTextsRequest.md) |  | 
**timer** | [**MaintenanceTimerRequest**](MaintenanceTimerRequest.md) |  | 
**social_networks** | [**MaintenanceSocialNetworksRequest**](MaintenanceSocialNetworksRequest.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.maintenance_preview_request import MaintenancePreviewRequest

# TODO update the JSON string below
json = "{}"
# create an instance of MaintenancePreviewRequest from a JSON string
maintenance_preview_request_instance = MaintenancePreviewRequest.from_json(json)
# print the JSON string representation of the object
print(MaintenancePreviewRequest.to_json())

# convert the object into a dict
maintenance_preview_request_dict = maintenance_preview_request_instance.to_dict()
# create an instance of MaintenancePreviewRequest from a dict
maintenance_preview_request_from_dict = MaintenancePreviewRequest.from_dict(maintenance_preview_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


