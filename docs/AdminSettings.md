# AdminSettings

Default settings of site administrator

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | [**AdminSettingsValue**](AdminSettingsValue.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.admin_settings import AdminSettings

# TODO update the JSON string below
json = "{}"
# create an instance of AdminSettings from a JSON string
admin_settings_instance = AdminSettings.from_json(json)
# print the JSON string representation of the object
print(AdminSettings.to_json())

# convert the object into a dict
admin_settings_dict = admin_settings_instance.to_dict()
# create an instance of AdminSettings from a dict
admin_settings_from_dict = AdminSettings.from_dict(admin_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


