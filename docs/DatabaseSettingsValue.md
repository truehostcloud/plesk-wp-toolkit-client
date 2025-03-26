# DatabaseSettingsValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | [**DatabaseSettingsValueName**](DatabaseSettingsValueName.md) |  | 
**server** | [**ParameterWithChoices**](ParameterWithChoices.md) |  | 
**user_name** | [**DatabaseSettingsValueUserName**](DatabaseSettingsValueUserName.md) |  | 
**user_password** | [**DatabaseSettingsValueUserPassword**](DatabaseSettingsValueUserPassword.md) |  | 
**table_prefix** | [**DatabaseSettingsValueTablePrefix**](DatabaseSettingsValueTablePrefix.md) |  | 
**name_prefix** | [**DatabaseSettingsValueNamePrefix**](DatabaseSettingsValueNamePrefix.md) |  | [optional] 
**user_name_prefix** | [**DatabaseSettingsValueUserNamePrefix**](DatabaseSettingsValueUserNamePrefix.md) |  | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.database_settings_value import DatabaseSettingsValue

# TODO update the JSON string below
json = "{}"
# create an instance of DatabaseSettingsValue from a JSON string
database_settings_value_instance = DatabaseSettingsValue.from_json(json)
# print the JSON string representation of the object
print(DatabaseSettingsValue.to_json())

# convert the object into a dict
database_settings_value_dict = database_settings_value_instance.to_dict()
# create an instance of DatabaseSettingsValue from a dict
database_settings_value_from_dict = DatabaseSettingsValue.from_dict(database_settings_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


