# InstallationCloneSubdomainSettingsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**parent_domain** | **str** | Domain name | 
**name** | **str** | Subdomain name | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_clone_subdomain_settings_request import InstallationCloneSubdomainSettingsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationCloneSubdomainSettingsRequest from a JSON string
installation_clone_subdomain_settings_request_instance = InstallationCloneSubdomainSettingsRequest.from_json(json)
# print the JSON string representation of the object
print(InstallationCloneSubdomainSettingsRequest.to_json())

# convert the object into a dict
installation_clone_subdomain_settings_request_dict = installation_clone_subdomain_settings_request_instance.to_dict()
# create an instance of InstallationCloneSubdomainSettingsRequest from a dict
installation_clone_subdomain_settings_request_from_dict = InstallationCloneSubdomainSettingsRequest.from_dict(installation_clone_subdomain_settings_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


