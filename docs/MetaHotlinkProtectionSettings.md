# MetaHotlinkProtectionSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | [**MetaHotlinkProtectionSettingsValue**](MetaHotlinkProtectionSettingsValue.md) |  | 
**meta** | **object** |  | 

## Example

```python
from plesk_wp_toolkit_client.models.meta_hotlink_protection_settings import MetaHotlinkProtectionSettings

# TODO update the JSON string below
json = "{}"
# create an instance of MetaHotlinkProtectionSettings from a JSON string
meta_hotlink_protection_settings_instance = MetaHotlinkProtectionSettings.from_json(json)
# print the JSON string representation of the object
print(MetaHotlinkProtectionSettings.to_json())

# convert the object into a dict
meta_hotlink_protection_settings_dict = meta_hotlink_protection_settings_instance.to_dict()
# create an instance of MetaHotlinkProtectionSettings from a dict
meta_hotlink_protection_settings_from_dict = MetaHotlinkProtectionSettings.from_dict(meta_hotlink_protection_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


