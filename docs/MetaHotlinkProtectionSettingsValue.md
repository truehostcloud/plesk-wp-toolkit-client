# MetaHotlinkProtectionSettingsValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**domains** | [**MetaHotlinkProtectionSettingsValueDomains**](MetaHotlinkProtectionSettingsValueDomains.md) |  | 
**file_extensions** | [**MetaHotlinkProtectionSettingsValueFileExtensions**](MetaHotlinkProtectionSettingsValueFileExtensions.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.meta_hotlink_protection_settings_value import MetaHotlinkProtectionSettingsValue

# TODO update the JSON string below
json = "{}"
# create an instance of MetaHotlinkProtectionSettingsValue from a JSON string
meta_hotlink_protection_settings_value_instance = MetaHotlinkProtectionSettingsValue.from_json(json)
# print the JSON string representation of the object
print(MetaHotlinkProtectionSettingsValue.to_json())

# convert the object into a dict
meta_hotlink_protection_settings_value_dict = meta_hotlink_protection_settings_value_instance.to_dict()
# create an instance of MetaHotlinkProtectionSettingsValue from a dict
meta_hotlink_protection_settings_value_from_dict = MetaHotlinkProtectionSettingsValue.from_dict(meta_hotlink_protection_settings_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


