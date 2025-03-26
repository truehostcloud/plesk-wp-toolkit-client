# InstallationSecurityPoliciesCoreSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**update_vulnerable** | **bool** | Update vulnerable WordPress core | [optional] 
**apply_virtual_patches** | **bool** | Apply virtual patches for WordPress core | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.installation_security_policies_core_settings import InstallationSecurityPoliciesCoreSettings

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationSecurityPoliciesCoreSettings from a JSON string
installation_security_policies_core_settings_instance = InstallationSecurityPoliciesCoreSettings.from_json(json)
# print the JSON string representation of the object
print(InstallationSecurityPoliciesCoreSettings.to_json())

# convert the object into a dict
installation_security_policies_core_settings_dict = installation_security_policies_core_settings_instance.to_dict()
# create an instance of InstallationSecurityPoliciesCoreSettings from a dict
installation_security_policies_core_settings_from_dict = InstallationSecurityPoliciesCoreSettings.from_dict(installation_security_policies_core_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


