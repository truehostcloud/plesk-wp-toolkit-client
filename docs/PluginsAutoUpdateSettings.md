# PluginsAutoUpdateSettings

Default plugin autoupdate settings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | [**PluginsAutoUpdateSettingsValue**](PluginsAutoUpdateSettingsValue.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.plugins_auto_update_settings import PluginsAutoUpdateSettings

# TODO update the JSON string below
json = "{}"
# create an instance of PluginsAutoUpdateSettings from a JSON string
plugins_auto_update_settings_instance = PluginsAutoUpdateSettings.from_json(json)
# print the JSON string representation of the object
print(PluginsAutoUpdateSettings.to_json())

# convert the object into a dict
plugins_auto_update_settings_dict = plugins_auto_update_settings_instance.to_dict()
# create an instance of PluginsAutoUpdateSettings from a dict
plugins_auto_update_settings_from_dict = PluginsAutoUpdateSettings.from_dict(plugins_auto_update_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


