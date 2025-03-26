# HotlinkProtectionStatusRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **bool** | Status | 

## Example

```python
from plesk_wp_toolkit_client.models.hotlink_protection_status_request import HotlinkProtectionStatusRequest

# TODO update the JSON string below
json = "{}"
# create an instance of HotlinkProtectionStatusRequest from a JSON string
hotlink_protection_status_request_instance = HotlinkProtectionStatusRequest.from_json(json)
# print the JSON string representation of the object
print(HotlinkProtectionStatusRequest.to_json())

# convert the object into a dict
hotlink_protection_status_request_dict = hotlink_protection_status_request_instance.to_dict()
# create an instance of HotlinkProtectionStatusRequest from a dict
hotlink_protection_status_request_from_dict = HotlinkProtectionStatusRequest.from_dict(hotlink_protection_status_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


