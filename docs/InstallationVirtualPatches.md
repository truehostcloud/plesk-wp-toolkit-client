# InstallationVirtualPatches


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **bool** | Whether the WordPress installation has vulnerability protection enabled or not | 
**available** | **bool** | Whether is feature available | 
**restrictions** | [**List[InstallationVirtualPatchesRestrictionsEnum]**](InstallationVirtualPatchesRestrictionsEnum.md) | List of restrictions for feature | 
**subscription** | [**InstallationVirtualPatchesSubscription**](InstallationVirtualPatchesSubscription.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_virtual_patches import InstallationVirtualPatches

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationVirtualPatches from a JSON string
installation_virtual_patches_instance = InstallationVirtualPatches.from_json(json)
# print the JSON string representation of the object
print(InstallationVirtualPatches.to_json())

# convert the object into a dict
installation_virtual_patches_dict = installation_virtual_patches_instance.to_dict()
# create an instance of InstallationVirtualPatches from a dict
installation_virtual_patches_from_dict = InstallationVirtualPatches.from_dict(installation_virtual_patches_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


