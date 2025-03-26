# AutoUpdateSettingsValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**core** | [**AutoUpdateSettingsValueCore**](AutoUpdateSettingsValueCore.md) |  | 
**plugins** | [**PluginsAutoUpdateSettings**](PluginsAutoUpdateSettings.md) |  | 
**themes** | [**ThemesAutoUpdateSettings**](ThemesAutoUpdateSettings.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.auto_update_settings_value import AutoUpdateSettingsValue

# TODO update the JSON string below
json = "{}"
# create an instance of AutoUpdateSettingsValue from a JSON string
auto_update_settings_value_instance = AutoUpdateSettingsValue.from_json(json)
# print the JSON string representation of the object
print(AutoUpdateSettingsValue.to_json())

# convert the object into a dict
auto_update_settings_value_dict = auto_update_settings_value_instance.to_dict()
# create an instance of AutoUpdateSettingsValue from a dict
auto_update_settings_value_from_dict = AutoUpdateSettingsValue.from_dict(auto_update_settings_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


