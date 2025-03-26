# ThemesAutoUpdateSettings

Default theme autoupdate settings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | [**ThemesAutoUpdateSettingsValue**](ThemesAutoUpdateSettingsValue.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.themes_auto_update_settings import ThemesAutoUpdateSettings

# TODO update the JSON string below
json = "{}"
# create an instance of ThemesAutoUpdateSettings from a JSON string
themes_auto_update_settings_instance = ThemesAutoUpdateSettings.from_json(json)
# print the JSON string representation of the object
print(ThemesAutoUpdateSettings.to_json())

# convert the object into a dict
themes_auto_update_settings_dict = themes_auto_update_settings_instance.to_dict()
# create an instance of ThemesAutoUpdateSettings from a dict
themes_auto_update_settings_from_dict = ThemesAutoUpdateSettings.from_dict(themes_auto_update_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


