# AutoUpdateSettings

Default autoupdate settings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | [**AutoUpdateSettingsValue**](AutoUpdateSettingsValue.md) |  | 
**meta** | [**AutoUpdateSettingsMeta**](AutoUpdateSettingsMeta.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.auto_update_settings import AutoUpdateSettings

# TODO update the JSON string below
json = "{}"
# create an instance of AutoUpdateSettings from a JSON string
auto_update_settings_instance = AutoUpdateSettings.from_json(json)
# print the JSON string representation of the object
print(AutoUpdateSettings.to_json())

# convert the object into a dict
auto_update_settings_dict = auto_update_settings_instance.to_dict()
# create an instance of AutoUpdateSettings from a dict
auto_update_settings_from_dict = AutoUpdateSettings.from_dict(auto_update_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


