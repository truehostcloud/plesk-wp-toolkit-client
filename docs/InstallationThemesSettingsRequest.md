# InstallationThemesSettingsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**force_updates** | **bool** | Update themes automatically | [optional] 
**newly_installed_updates** | **bool** | Enable autoupdates by default for new themes | [optional] 
**update_vulnerable** | **bool** | Autoupdate vulnerable themes | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.installation_themes_settings_request import InstallationThemesSettingsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationThemesSettingsRequest from a JSON string
installation_themes_settings_request_instance = InstallationThemesSettingsRequest.from_json(json)
# print the JSON string representation of the object
print(InstallationThemesSettingsRequest.to_json())

# convert the object into a dict
installation_themes_settings_request_dict = installation_themes_settings_request_instance.to_dict()
# create an instance of InstallationThemesSettingsRequest from a dict
installation_themes_settings_request_from_dict = InstallationThemesSettingsRequest.from_dict(installation_themes_settings_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


