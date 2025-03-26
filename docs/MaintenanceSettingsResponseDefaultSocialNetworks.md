# MaintenanceSettingsResponseDefaultSocialNetworks

Default links to your social network pages

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**facebook** | **str** | Link to Facebook | 
**twitter** | **str** | Link to Twitter | 
**instagram** | **str** | Link to Instagram | 

## Example

```python
from plesk_wp_toolkit_client.models.maintenance_settings_response_default_social_networks import MaintenanceSettingsResponseDefaultSocialNetworks

# TODO update the JSON string below
json = "{}"
# create an instance of MaintenanceSettingsResponseDefaultSocialNetworks from a JSON string
maintenance_settings_response_default_social_networks_instance = MaintenanceSettingsResponseDefaultSocialNetworks.from_json(json)
# print the JSON string representation of the object
print(MaintenanceSettingsResponseDefaultSocialNetworks.to_json())

# convert the object into a dict
maintenance_settings_response_default_social_networks_dict = maintenance_settings_response_default_social_networks_instance.to_dict()
# create an instance of MaintenanceSettingsResponseDefaultSocialNetworks from a dict
maintenance_settings_response_default_social_networks_from_dict = MaintenanceSettingsResponseDefaultSocialNetworks.from_dict(maintenance_settings_response_default_social_networks_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


