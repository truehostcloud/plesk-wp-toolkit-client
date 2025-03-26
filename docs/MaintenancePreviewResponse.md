# MaintenancePreviewResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **str** | URL to the maintenance mode preview | 

## Example

```python
from plesk_wp_toolkit_client.models.maintenance_preview_response import MaintenancePreviewResponse

# TODO update the JSON string below
json = "{}"
# create an instance of MaintenancePreviewResponse from a JSON string
maintenance_preview_response_instance = MaintenancePreviewResponse.from_json(json)
# print the JSON string representation of the object
print(MaintenancePreviewResponse.to_json())

# convert the object into a dict
maintenance_preview_response_dict = maintenance_preview_response_instance.to_dict()
# create an instance of MaintenancePreviewResponse from a dict
maintenance_preview_response_from_dict = MaintenancePreviewResponse.from_dict(maintenance_preview_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


