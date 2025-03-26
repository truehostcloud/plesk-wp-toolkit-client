# MaintenanceSettingsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**full_mode** | **bool** | Allow access to WordPress admin dashboard when maintenance mode is enabled | 
**texts** | [**MaintenanceTextsRequest**](MaintenanceTextsRequest.md) |  | 
**timer** | [**MaintenanceTimerRequest**](MaintenanceTimerRequest.md) |  | 
**social_networks** | [**MaintenanceSocialNetworksRequest**](MaintenanceSocialNetworksRequest.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.maintenance_settings_request import MaintenanceSettingsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of MaintenanceSettingsRequest from a JSON string
maintenance_settings_request_instance = MaintenanceSettingsRequest.from_json(json)
# print the JSON string representation of the object
print(MaintenanceSettingsRequest.to_json())

# convert the object into a dict
maintenance_settings_request_dict = maintenance_settings_request_instance.to_dict()
# create an instance of MaintenanceSettingsRequest from a dict
maintenance_settings_request_from_dict = MaintenanceSettingsRequest.from_dict(maintenance_settings_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


