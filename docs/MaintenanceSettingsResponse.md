# MaintenanceSettingsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**full_mode** | **bool** | Allow access to WordPress admin dashboard when maintance mode is enabled | 
**texts** | [**MaintenanceSettingsResponseTexts**](MaintenanceSettingsResponseTexts.md) |  | 
**timer** | [**MaintenanceSettingsResponseTimer**](MaintenanceSettingsResponseTimer.md) |  | 
**social_networks** | [**MaintenanceSettingsResponseSocialNetworks**](MaintenanceSettingsResponseSocialNetworks.md) |  | 
**default_social_networks** | [**MaintenanceSettingsResponseDefaultSocialNetworks**](MaintenanceSettingsResponseDefaultSocialNetworks.md) |  | 
**template_file_path** | **str** | Path to the maintenance mode template | 

## Example

```python
from plesk_wp_toolkit_client.models.maintenance_settings_response import MaintenanceSettingsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of MaintenanceSettingsResponse from a JSON string
maintenance_settings_response_instance = MaintenanceSettingsResponse.from_json(json)
# print the JSON string representation of the object
print(MaintenanceSettingsResponse.to_json())

# convert the object into a dict
maintenance_settings_response_dict = maintenance_settings_response_instance.to_dict()
# create an instance of MaintenanceSettingsResponse from a dict
maintenance_settings_response_from_dict = MaintenanceSettingsResponse.from_dict(maintenance_settings_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


