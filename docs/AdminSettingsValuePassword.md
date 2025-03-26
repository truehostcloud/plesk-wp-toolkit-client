# AdminSettingsValuePassword

Site administrator password

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **str** |  | 

## Example

```python
from plesk_wp_toolkit_client.models.admin_settings_value_password import AdminSettingsValuePassword

# TODO update the JSON string below
json = "{}"
# create an instance of AdminSettingsValuePassword from a JSON string
admin_settings_value_password_instance = AdminSettingsValuePassword.from_json(json)
# print the JSON string representation of the object
print(AdminSettingsValuePassword.to_json())

# convert the object into a dict
admin_settings_value_password_dict = admin_settings_value_password_instance.to_dict()
# create an instance of AdminSettingsValuePassword from a dict
admin_settings_value_password_from_dict = AdminSettingsValuePassword.from_dict(admin_settings_value_password_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


