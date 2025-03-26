# InstallationThemesSettingsResponse

Theme autoupdate settings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**force_updates** | **bool** | Update themes automatically | 
**newly_installed_updates** | **bool** | Enable autoupdates by default for new themes | 
**update_vulnerable** | **bool** | Autoupdate vulnerable themes | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_themes_settings_response import InstallationThemesSettingsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationThemesSettingsResponse from a JSON string
installation_themes_settings_response_instance = InstallationThemesSettingsResponse.from_json(json)
# print the JSON string representation of the object
print(InstallationThemesSettingsResponse.to_json())

# convert the object into a dict
installation_themes_settings_response_dict = installation_themes_settings_response_instance.to_dict()
# create an instance of InstallationThemesSettingsResponse from a dict
installation_themes_settings_response_from_dict = InstallationThemesSettingsResponse.from_dict(installation_themes_settings_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


