# InstallationPluginsSettingsResponse

Plugin autoupdate settings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**force_updates** | **bool** | Update plugins automatically | 
**newly_installed_updates** | **bool** | Enable autoupdates by default for new plugins | 
**update_vulnerable** | **bool** | Autoupdate vulnerable plugins | 
**deactivate_vulnerable** | **bool** | Deactivate vulnerable plugins | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_plugins_settings_response import InstallationPluginsSettingsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationPluginsSettingsResponse from a JSON string
installation_plugins_settings_response_instance = InstallationPluginsSettingsResponse.from_json(json)
# print the JSON string representation of the object
print(InstallationPluginsSettingsResponse.to_json())

# convert the object into a dict
installation_plugins_settings_response_dict = installation_plugins_settings_response_instance.to_dict()
# create an instance of InstallationPluginsSettingsResponse from a dict
installation_plugins_settings_response_from_dict = InstallationPluginsSettingsResponse.from_dict(installation_plugins_settings_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


