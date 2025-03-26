# VirtualPatchesInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**installations_limit** | **int** | Maximum number of WordPress installations that can use vulnerability protection (according to license limits) | 
**installations_active** | **int** | Current number of WordPress installations with enabled vulnerability protection | 

## Example

```python
from plesk_wp_toolkit_client.models.virtual_patches_info import VirtualPatchesInfo

# TODO update the JSON string below
json = "{}"
# create an instance of VirtualPatchesInfo from a JSON string
virtual_patches_info_instance = VirtualPatchesInfo.from_json(json)
# print the JSON string representation of the object
print(VirtualPatchesInfo.to_json())

# convert the object into a dict
virtual_patches_info_dict = virtual_patches_info_instance.to_dict()
# create an instance of VirtualPatchesInfo from a dict
virtual_patches_info_from_dict = VirtualPatchesInfo.from_dict(virtual_patches_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


