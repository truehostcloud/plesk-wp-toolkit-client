# InstallationCloneRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**installation_id** | **int** | Installation ID | 
**domain** | [**InstallationCloneDomainSettingsRequest**](InstallationCloneDomainSettingsRequest.md) |  | 
**installation_path** | **str** | Installation path (relative to the root directory of the domain) | [optional] 
**overwrite** | **bool** | Overwrite installation | [optional] 
**database** | [**InstallationCloneDatabaseSettingsRequest**](InstallationCloneDatabaseSettingsRequest.md) |  | 
**show_domain_overview_link_on_done** | **bool** | Show overview link for background task | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.installation_clone_request import InstallationCloneRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationCloneRequest from a JSON string
installation_clone_request_instance = InstallationCloneRequest.from_json(json)
# print the JSON string representation of the object
print(InstallationCloneRequest.to_json())

# convert the object into a dict
installation_clone_request_dict = installation_clone_request_instance.to_dict()
# create an instance of InstallationCloneRequest from a dict
installation_clone_request_from_dict = InstallationCloneRequest.from_dict(installation_clone_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


