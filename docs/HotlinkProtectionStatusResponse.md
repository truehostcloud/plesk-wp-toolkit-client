# HotlinkProtectionStatusResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **bool** | Status | 

## Example

```python
from plesk_wp_toolkit_client.models.hotlink_protection_status_response import HotlinkProtectionStatusResponse

# TODO update the JSON string below
json = "{}"
# create an instance of HotlinkProtectionStatusResponse from a JSON string
hotlink_protection_status_response_instance = HotlinkProtectionStatusResponse.from_json(json)
# print the JSON string representation of the object
print(HotlinkProtectionStatusResponse.to_json())

# convert the object into a dict
hotlink_protection_status_response_dict = hotlink_protection_status_response_instance.to_dict()
# create an instance of HotlinkProtectionStatusResponse from a dict
hotlink_protection_status_response_from_dict = HotlinkProtectionStatusResponse.from_dict(hotlink_protection_status_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


