# AdminSettingsValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**login** | [**AdminSettingsValueLogin**](AdminSettingsValueLogin.md) |  | 
**password** | [**AdminSettingsValuePassword**](AdminSettingsValuePassword.md) |  | 
**email** | [**AdminSettingsValueEmail**](AdminSettingsValueEmail.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.admin_settings_value import AdminSettingsValue

# TODO update the JSON string below
json = "{}"
# create an instance of AdminSettingsValue from a JSON string
admin_settings_value_instance = AdminSettingsValue.from_json(json)
# print the JSON string representation of the object
print(AdminSettingsValue.to_json())

# convert the object into a dict
admin_settings_value_dict = admin_settings_value_instance.to_dict()
# create an instance of AdminSettingsValue from a dict
admin_settings_value_from_dict = AdminSettingsValue.from_dict(admin_settings_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


