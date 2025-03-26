# AdminSettingsValueEmail

Site administrator e-mail

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **str** |  | 

## Example

```python
from plesk_wp_toolkit_client.models.admin_settings_value_email import AdminSettingsValueEmail

# TODO update the JSON string below
json = "{}"
# create an instance of AdminSettingsValueEmail from a JSON string
admin_settings_value_email_instance = AdminSettingsValueEmail.from_json(json)
# print the JSON string representation of the object
print(AdminSettingsValueEmail.to_json())

# convert the object into a dict
admin_settings_value_email_dict = admin_settings_value_email_instance.to_dict()
# create an instance of AdminSettingsValueEmail from a dict
admin_settings_value_email_from_dict = AdminSettingsValueEmail.from_dict(admin_settings_value_email_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


