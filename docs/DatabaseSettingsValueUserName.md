# DatabaseSettingsValueUserName

Database user name

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **str** |  | 

## Example

```python
from plesk_wp_toolkit_client.models.database_settings_value_user_name import DatabaseSettingsValueUserName

# TODO update the JSON string below
json = "{}"
# create an instance of DatabaseSettingsValueUserName from a JSON string
database_settings_value_user_name_instance = DatabaseSettingsValueUserName.from_json(json)
# print the JSON string representation of the object
print(DatabaseSettingsValueUserName.to_json())

# convert the object into a dict
database_settings_value_user_name_dict = database_settings_value_user_name_instance.to_dict()
# create an instance of DatabaseSettingsValueUserName from a dict
database_settings_value_user_name_from_dict = DatabaseSettingsValueUserName.from_dict(database_settings_value_user_name_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


