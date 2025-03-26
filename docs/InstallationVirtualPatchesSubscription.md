# InstallationVirtualPatchesSubscription


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | [**InstallationVirtualPatchesSubscriptionStatusEnum**](InstallationVirtualPatchesSubscriptionStatusEnum.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_virtual_patches_subscription import InstallationVirtualPatchesSubscription

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationVirtualPatchesSubscription from a JSON string
installation_virtual_patches_subscription_instance = InstallationVirtualPatchesSubscription.from_json(json)
# print the JSON string representation of the object
print(InstallationVirtualPatchesSubscription.to_json())

# convert the object into a dict
installation_virtual_patches_subscription_dict = installation_virtual_patches_subscription_instance.to_dict()
# create an instance of InstallationVirtualPatchesSubscription from a dict
installation_virtual_patches_subscription_from_dict = InstallationVirtualPatchesSubscription.from_dict(installation_virtual_patches_subscription_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


