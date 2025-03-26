# LicenseInfoResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**virtual_patches** | [**LicenseInfoResponseVirtualPatches**](LicenseInfoResponseVirtualPatches.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.license_info_response import LicenseInfoResponse

# TODO update the JSON string below
json = "{}"
# create an instance of LicenseInfoResponse from a JSON string
license_info_response_instance = LicenseInfoResponse.from_json(json)
# print the JSON string representation of the object
print(LicenseInfoResponse.to_json())

# convert the object into a dict
license_info_response_dict = license_info_response_instance.to_dict()
# create an instance of LicenseInfoResponse from a dict
license_info_response_from_dict = LicenseInfoResponse.from_dict(license_info_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


