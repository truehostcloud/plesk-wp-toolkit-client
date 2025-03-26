# LicenseInfoResponseVirtualPatches

Vulnerability protection information

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**installations_limit** | **int** | Maximum number of WordPress installations that can use vulnerability protection (according to license limits) | 
**installations_active** | **int** | Current number of WordPress installations with enabled vulnerability protection | 

## Example

```python
from plesk_wp_toolkit_client.models.license_info_response_virtual_patches import LicenseInfoResponseVirtualPatches

# TODO update the JSON string below
json = "{}"
# create an instance of LicenseInfoResponseVirtualPatches from a JSON string
license_info_response_virtual_patches_instance = LicenseInfoResponseVirtualPatches.from_json(json)
# print the JSON string representation of the object
print(LicenseInfoResponseVirtualPatches.to_json())

# convert the object into a dict
license_info_response_virtual_patches_dict = license_info_response_virtual_patches_instance.to_dict()
# create an instance of LicenseInfoResponseVirtualPatches from a dict
license_info_response_virtual_patches_from_dict = LicenseInfoResponseVirtualPatches.from_dict(license_info_response_virtual_patches_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


