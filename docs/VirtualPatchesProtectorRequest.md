# VirtualPatchesProtectorRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**installations_ids** | **List[int]** |  | 
**status** | **bool** | Whether the WordPress installation has vulnerability protection enabled or not | 
**skip_broken_installations** | **bool** | Ignore broken installations (by default request fails on them) | [optional] 
**skip_infected_installations** | **bool** | Ignore quarantined installations (by default request fails on them) | [optional] 
**skip_unsupported_installations** | **bool** | Ignore unsupported installations (by default request fails on them) | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.virtual_patches_protector_request import VirtualPatchesProtectorRequest

# TODO update the JSON string below
json = "{}"
# create an instance of VirtualPatchesProtectorRequest from a JSON string
virtual_patches_protector_request_instance = VirtualPatchesProtectorRequest.from_json(json)
# print the JSON string representation of the object
print(VirtualPatchesProtectorRequest.to_json())

# convert the object into a dict
virtual_patches_protector_request_dict = virtual_patches_protector_request_instance.to_dict()
# create an instance of VirtualPatchesProtectorRequest from a dict
virtual_patches_protector_request_from_dict = VirtualPatchesProtectorRequest.from_dict(virtual_patches_protector_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


