# DatabaseSettingsValueName

Database name

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **str** |  | 
**meta** | [**AutoUpdateSettingsMeta**](AutoUpdateSettingsMeta.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.database_settings_value_name import DatabaseSettingsValueName

# TODO update the JSON string below
json = "{}"
# create an instance of DatabaseSettingsValueName from a JSON string
database_settings_value_name_instance = DatabaseSettingsValueName.from_json(json)
# print the JSON string representation of the object
print(DatabaseSettingsValueName.to_json())

# convert the object into a dict
database_settings_value_name_dict = database_settings_value_name_instance.to_dict()
# create an instance of DatabaseSettingsValueName from a dict
database_settings_value_name_from_dict = DatabaseSettingsValueName.from_dict(database_settings_value_name_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


