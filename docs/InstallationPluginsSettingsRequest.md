# InstallationPluginsSettingsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**force_updates** | **bool** | Update plugins automatically | [optional] 
**newly_installed_updates** | **bool** | Enable autoupdates by default for new plugins | [optional] 
**update_vulnerable** | **bool** | Autoupdate vulnerable plugins | [optional] 
**deactivate_vulnerable** | **bool** | Deactivate vulnerable plugins | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.installation_plugins_settings_request import InstallationPluginsSettingsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationPluginsSettingsRequest from a JSON string
installation_plugins_settings_request_instance = InstallationPluginsSettingsRequest.from_json(json)
# print the JSON string representation of the object
print(InstallationPluginsSettingsRequest.to_json())

# convert the object into a dict
installation_plugins_settings_request_dict = installation_plugins_settings_request_instance.to_dict()
# create an instance of InstallationPluginsSettingsRequest from a dict
installation_plugins_settings_request_from_dict = InstallationPluginsSettingsRequest.from_dict(installation_plugins_settings_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


