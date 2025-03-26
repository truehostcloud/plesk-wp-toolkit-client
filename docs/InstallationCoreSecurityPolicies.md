# InstallationCoreSecurityPolicies

Core security policies settings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**update_vulnerable** | **bool** | Update WordPress core automatically | 
**apply_virtual_patches** | **bool** | Apply virtual patches for WordPress core | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_core_security_policies import InstallationCoreSecurityPolicies

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationCoreSecurityPolicies from a JSON string
installation_core_security_policies_instance = InstallationCoreSecurityPolicies.from_json(json)
# print the JSON string representation of the object
print(InstallationCoreSecurityPolicies.to_json())

# convert the object into a dict
installation_core_security_policies_dict = installation_core_security_policies_instance.to_dict()
# create an instance of InstallationCoreSecurityPolicies from a dict
installation_core_security_policies_from_dict = InstallationCoreSecurityPolicies.from_dict(installation_core_security_policies_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


