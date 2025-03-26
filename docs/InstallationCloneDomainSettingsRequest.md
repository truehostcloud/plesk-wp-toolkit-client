# InstallationCloneDomainSettingsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**existing** | **str** | Domain name | [optional] 
**new_subdomain** | [**InstallationCloneSubdomainSettingsRequest**](InstallationCloneSubdomainSettingsRequest.md) |  | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.installation_clone_domain_settings_request import InstallationCloneDomainSettingsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationCloneDomainSettingsRequest from a JSON string
installation_clone_domain_settings_request_instance = InstallationCloneDomainSettingsRequest.from_json(json)
# print the JSON string representation of the object
print(InstallationCloneDomainSettingsRequest.to_json())

# convert the object into a dict
installation_clone_domain_settings_request_dict = installation_clone_domain_settings_request_instance.to_dict()
# create an instance of InstallationCloneDomainSettingsRequest from a dict
installation_clone_domain_settings_request_from_dict = InstallationCloneDomainSettingsRequest.from_dict(installation_clone_domain_settings_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


