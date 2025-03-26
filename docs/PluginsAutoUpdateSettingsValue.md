# PluginsAutoUpdateSettingsValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**force_updates** | [**PluginsAutoUpdateSettingsValueForceUpdates**](PluginsAutoUpdateSettingsValueForceUpdates.md) |  | 
**newly_installed_updates** | [**PluginsAutoUpdateSettingsValueNewlyInstalledUpdates**](PluginsAutoUpdateSettingsValueNewlyInstalledUpdates.md) |  | 
**update_vulnerable** | [**PluginsAutoUpdateSettingsValueUpdateVulnerable**](PluginsAutoUpdateSettingsValueUpdateVulnerable.md) |  | 
**deactivate_vulnerable** | [**PluginsAutoUpdateSettingsValueDeactivateVulnerable**](PluginsAutoUpdateSettingsValueDeactivateVulnerable.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.plugins_auto_update_settings_value import PluginsAutoUpdateSettingsValue

# TODO update the JSON string below
json = "{}"
# create an instance of PluginsAutoUpdateSettingsValue from a JSON string
plugins_auto_update_settings_value_instance = PluginsAutoUpdateSettingsValue.from_json(json)
# print the JSON string representation of the object
print(PluginsAutoUpdateSettingsValue.to_json())

# convert the object into a dict
plugins_auto_update_settings_value_dict = plugins_auto_update_settings_value_instance.to_dict()
# create an instance of PluginsAutoUpdateSettingsValue from a dict
plugins_auto_update_settings_value_from_dict = PluginsAutoUpdateSettingsValue.from_dict(plugins_auto_update_settings_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


