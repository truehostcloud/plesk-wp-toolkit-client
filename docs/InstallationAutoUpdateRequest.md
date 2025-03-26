# InstallationAutoUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**core** | **str** | WordPress core autoupdate settings | [optional] 
**plugins** | [**InstallationPluginsSettingsRequest**](InstallationPluginsSettingsRequest.md) |  | [optional] 
**themes** | [**InstallationThemesSettingsRequest**](InstallationThemesSettingsRequest.md) |  | [optional] 
**safe_update** | **bool** | Enable creation of backup during updating | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.installation_auto_update_request import InstallationAutoUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationAutoUpdateRequest from a JSON string
installation_auto_update_request_instance = InstallationAutoUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(InstallationAutoUpdateRequest.to_json())

# convert the object into a dict
installation_auto_update_request_dict = installation_auto_update_request_instance.to_dict()
# create an instance of InstallationAutoUpdateRequest from a dict
installation_auto_update_request_from_dict = InstallationAutoUpdateRequest.from_dict(installation_auto_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


