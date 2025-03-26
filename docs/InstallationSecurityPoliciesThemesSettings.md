# InstallationSecurityPoliciesThemesSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**update_vulnerable** | **bool** | Autoupdate vulnerable themes | [optional] 
**apply_virtual_patches** | **bool** | Apply virtual patches for vulnerable plugins | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.installation_security_policies_themes_settings import InstallationSecurityPoliciesThemesSettings

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationSecurityPoliciesThemesSettings from a JSON string
installation_security_policies_themes_settings_instance = InstallationSecurityPoliciesThemesSettings.from_json(json)
# print the JSON string representation of the object
print(InstallationSecurityPoliciesThemesSettings.to_json())

# convert the object into a dict
installation_security_policies_themes_settings_dict = installation_security_policies_themes_settings_instance.to_dict()
# create an instance of InstallationSecurityPoliciesThemesSettings from a dict
installation_security_policies_themes_settings_from_dict = InstallationSecurityPoliciesThemesSettings.from_dict(installation_security_policies_themes_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


