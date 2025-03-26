# MetaHotlinkProtectionSettingsValueDomains


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | [**List[MetaHotlinkProtectionSettingsDomainsValue]**](MetaHotlinkProtectionSettingsDomainsValue.md) |  | 
**meta** | [**MetaHotlinkProtectionSettingsValueDomainsMeta**](MetaHotlinkProtectionSettingsValueDomainsMeta.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.meta_hotlink_protection_settings_value_domains import MetaHotlinkProtectionSettingsValueDomains

# TODO update the JSON string below
json = "{}"
# create an instance of MetaHotlinkProtectionSettingsValueDomains from a JSON string
meta_hotlink_protection_settings_value_domains_instance = MetaHotlinkProtectionSettingsValueDomains.from_json(json)
# print the JSON string representation of the object
print(MetaHotlinkProtectionSettingsValueDomains.to_json())

# convert the object into a dict
meta_hotlink_protection_settings_value_domains_dict = meta_hotlink_protection_settings_value_domains_instance.to_dict()
# create an instance of MetaHotlinkProtectionSettingsValueDomains from a dict
meta_hotlink_protection_settings_value_domains_from_dict = MetaHotlinkProtectionSettingsValueDomains.from_dict(meta_hotlink_protection_settings_value_domains_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


