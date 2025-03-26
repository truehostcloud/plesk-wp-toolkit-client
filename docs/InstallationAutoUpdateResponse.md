# InstallationAutoUpdateResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available** | **bool** | Availability of autoupdates feature | 
**safe_update** | **bool** | Enable creation of backup during updating | 
**core** | **str** | Update WordPress core automatically | 
**plugins** | [**InstallationPluginsSettingsResponse**](InstallationPluginsSettingsResponse.md) |  | 
**themes** | [**InstallationThemesSettingsResponse**](InstallationThemesSettingsResponse.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_auto_update_response import InstallationAutoUpdateResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationAutoUpdateResponse from a JSON string
installation_auto_update_response_instance = InstallationAutoUpdateResponse.from_json(json)
# print the JSON string representation of the object
print(InstallationAutoUpdateResponse.to_json())

# convert the object into a dict
installation_auto_update_response_dict = installation_auto_update_response_instance.to_dict()
# create an instance of InstallationAutoUpdateResponse from a dict
installation_auto_update_response_from_dict = InstallationAutoUpdateResponse.from_dict(installation_auto_update_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


