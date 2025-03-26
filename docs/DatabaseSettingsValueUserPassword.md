# DatabaseSettingsValueUserPassword

Database user password

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **str** |  | 

## Example

```python
from plesk_wp_toolkit_client.models.database_settings_value_user_password import DatabaseSettingsValueUserPassword

# TODO update the JSON string below
json = "{}"
# create an instance of DatabaseSettingsValueUserPassword from a JSON string
database_settings_value_user_password_instance = DatabaseSettingsValueUserPassword.from_json(json)
# print the JSON string representation of the object
print(DatabaseSettingsValueUserPassword.to_json())

# convert the object into a dict
database_settings_value_user_password_dict = database_settings_value_user_password_instance.to_dict()
# create an instance of DatabaseSettingsValueUserPassword from a dict
database_settings_value_user_password_from_dict = DatabaseSettingsValueUserPassword.from_dict(database_settings_value_user_password_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


