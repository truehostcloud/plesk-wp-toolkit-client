# InstallationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**domain** | **str** | Domain name | 
**installation_path** | **str** | Installation path relative to the root directory of the domain | [optional] 
**language** | **str** | Website language | [optional] 
**overwrite** | **bool** | Overwrite installation | [optional] 
**protocol** | **str** | Communication protocol | [optional] 
**set** | **int** | Set ID | [optional] 
**title** | **str** | Website title | [optional] 
**version** | **str** | WordPress version | [optional] 
**admin** | [**InstallationAdminSettingsRequest**](InstallationAdminSettingsRequest.md) |  | [optional] 
**database** | [**InstallationDatabaseSettingsRequest**](InstallationDatabaseSettingsRequest.md) |  | [optional] 
**auto_update** | [**InstallationAutoUpdateRequest**](InstallationAutoUpdateRequest.md) |  | [optional] 
**show_domain_overview_link_on_done** | **bool** | Show domain overview link in background task | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.installation_request import InstallationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationRequest from a JSON string
installation_request_instance = InstallationRequest.from_json(json)
# print the JSON string representation of the object
print(InstallationRequest.to_json())

# convert the object into a dict
installation_request_dict = installation_request_instance.to_dict()
# create an instance of InstallationRequest from a dict
installation_request_from_dict = InstallationRequest.from_dict(installation_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


