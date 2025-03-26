# InstallationSecurityPoliciesUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**core** | [**InstallationSecurityPoliciesCoreSettings**](InstallationSecurityPoliciesCoreSettings.md) |  | [optional] 
**plugins** | [**InstallationSecurityPoliciesPluginsSettings**](InstallationSecurityPoliciesPluginsSettings.md) |  | [optional] 
**themes** | [**InstallationSecurityPoliciesThemesSettings**](InstallationSecurityPoliciesThemesSettings.md) |  | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.installation_security_policies_update_request import InstallationSecurityPoliciesUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationSecurityPoliciesUpdateRequest from a JSON string
installation_security_policies_update_request_instance = InstallationSecurityPoliciesUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(InstallationSecurityPoliciesUpdateRequest.to_json())

# convert the object into a dict
installation_security_policies_update_request_dict = installation_security_policies_update_request_instance.to_dict()
# create an instance of InstallationSecurityPoliciesUpdateRequest from a dict
installation_security_policies_update_request_from_dict = InstallationSecurityPoliciesUpdateRequest.from_dict(installation_security_policies_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


