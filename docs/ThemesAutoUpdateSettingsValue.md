# ThemesAutoUpdateSettingsValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**force_updates** | [**ThemesAutoUpdateSettingsValueForceUpdates**](ThemesAutoUpdateSettingsValueForceUpdates.md) |  | 
**newly_installed_updates** | [**ThemesAutoUpdateSettingsValueNewlyInstalledUpdates**](ThemesAutoUpdateSettingsValueNewlyInstalledUpdates.md) |  | 
**update_vulnerable** | [**ThemesAutoUpdateSettingsValueUpdateVulnerable**](ThemesAutoUpdateSettingsValueUpdateVulnerable.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.themes_auto_update_settings_value import ThemesAutoUpdateSettingsValue

# TODO update the JSON string below
json = "{}"
# create an instance of ThemesAutoUpdateSettingsValue from a JSON string
themes_auto_update_settings_value_instance = ThemesAutoUpdateSettingsValue.from_json(json)
# print the JSON string representation of the object
print(ThemesAutoUpdateSettingsValue.to_json())

# convert the object into a dict
themes_auto_update_settings_value_dict = themes_auto_update_settings_value_instance.to_dict()
# create an instance of ThemesAutoUpdateSettingsValue from a dict
themes_auto_update_settings_value_from_dict = ThemesAutoUpdateSettingsValue.from_dict(themes_auto_update_settings_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


