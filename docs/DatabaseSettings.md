# DatabaseSettings

Default database settings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | [**DatabaseSettingsValue**](DatabaseSettingsValue.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.database_settings import DatabaseSettings

# TODO update the JSON string below
json = "{}"
# create an instance of DatabaseSettings from a JSON string
database_settings_instance = DatabaseSettings.from_json(json)
# print the JSON string representation of the object
print(DatabaseSettings.to_json())

# convert the object into a dict
database_settings_dict = database_settings_instance.to_dict()
# create an instance of DatabaseSettings from a dict
database_settings_from_dict = DatabaseSettings.from_dict(database_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


