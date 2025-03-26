# InstallationSecurityPoliciesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**core** | [**InstallationCoreSecurityPolicies**](InstallationCoreSecurityPolicies.md) |  | 
**plugins** | [**InstallationPluginsSettingsResponse**](InstallationPluginsSettingsResponse.md) |  | 
**themes** | [**InstallationThemesSettingsResponse**](InstallationThemesSettingsResponse.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_security_policies_response import InstallationSecurityPoliciesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationSecurityPoliciesResponse from a JSON string
installation_security_policies_response_instance = InstallationSecurityPoliciesResponse.from_json(json)
# print the JSON string representation of the object
print(InstallationSecurityPoliciesResponse.to_json())

# convert the object into a dict
installation_security_policies_response_dict = installation_security_policies_response_instance.to_dict()
# create an instance of InstallationSecurityPoliciesResponse from a dict
installation_security_policies_response_from_dict = InstallationSecurityPoliciesResponse.from_dict(installation_security_policies_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


