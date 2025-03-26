# HotlinkProtectionSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**domains** | **List[str]** | List of allowed domains | 
**file_extensions** | **List[str]** | List of allowed file extensions | 

## Example

```python
from plesk_wp_toolkit_client.models.hotlink_protection_settings import HotlinkProtectionSettings

# TODO update the JSON string below
json = "{}"
# create an instance of HotlinkProtectionSettings from a JSON string
hotlink_protection_settings_instance = HotlinkProtectionSettings.from_json(json)
# print the JSON string representation of the object
print(HotlinkProtectionSettings.to_json())

# convert the object into a dict
hotlink_protection_settings_dict = hotlink_protection_settings_instance.to_dict()
# create an instance of HotlinkProtectionSettings from a dict
hotlink_protection_settings_from_dict = HotlinkProtectionSettings.from_dict(hotlink_protection_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


