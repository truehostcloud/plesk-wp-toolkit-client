# AdminSettingsValueLogin

Site administrator username

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **str** |  | 

## Example

```python
from plesk_wp_toolkit_client.models.admin_settings_value_login import AdminSettingsValueLogin

# TODO update the JSON string below
json = "{}"
# create an instance of AdminSettingsValueLogin from a JSON string
admin_settings_value_login_instance = AdminSettingsValueLogin.from_json(json)
# print the JSON string representation of the object
print(AdminSettingsValueLogin.to_json())

# convert the object into a dict
admin_settings_value_login_dict = admin_settings_value_login_instance.to_dict()
# create an instance of AdminSettingsValueLogin from a dict
admin_settings_value_login_from_dict = AdminSettingsValueLogin.from_dict(admin_settings_value_login_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


