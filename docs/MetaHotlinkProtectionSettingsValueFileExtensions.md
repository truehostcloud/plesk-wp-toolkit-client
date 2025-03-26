# MetaHotlinkProtectionSettingsValueFileExtensions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | [**List[MetaHotlinkProtectionSettingsFileExtensionsValue]**](MetaHotlinkProtectionSettingsFileExtensionsValue.md) |  | 
**meta** | [**MetaHotlinkProtectionSettingsFileExtensionsMeta**](MetaHotlinkProtectionSettingsFileExtensionsMeta.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.meta_hotlink_protection_settings_value_file_extensions import MetaHotlinkProtectionSettingsValueFileExtensions

# TODO update the JSON string below
json = "{}"
# create an instance of MetaHotlinkProtectionSettingsValueFileExtensions from a JSON string
meta_hotlink_protection_settings_value_file_extensions_instance = MetaHotlinkProtectionSettingsValueFileExtensions.from_json(json)
# print the JSON string representation of the object
print(MetaHotlinkProtectionSettingsValueFileExtensions.to_json())

# convert the object into a dict
meta_hotlink_protection_settings_value_file_extensions_dict = meta_hotlink_protection_settings_value_file_extensions_instance.to_dict()
# create an instance of MetaHotlinkProtectionSettingsValueFileExtensions from a dict
meta_hotlink_protection_settings_value_file_extensions_from_dict = MetaHotlinkProtectionSettingsValueFileExtensions.from_dict(meta_hotlink_protection_settings_value_file_extensions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


