# AutoUpdateSettingsMeta


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**is_customization_allowed** | **bool** |  | 

## Example

```python
from plesk_wp_toolkit_client.models.auto_update_settings_meta import AutoUpdateSettingsMeta

# TODO update the JSON string below
json = "{}"
# create an instance of AutoUpdateSettingsMeta from a JSON string
auto_update_settings_meta_instance = AutoUpdateSettingsMeta.from_json(json)
# print the JSON string representation of the object
print(AutoUpdateSettingsMeta.to_json())

# convert the object into a dict
auto_update_settings_meta_dict = auto_update_settings_meta_instance.to_dict()
# create an instance of AutoUpdateSettingsMeta from a dict
auto_update_settings_meta_from_dict = AutoUpdateSettingsMeta.from_dict(auto_update_settings_meta_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


