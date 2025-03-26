# InstallationAdminSettingsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **str** | Site admin e-mail | [optional] 
**login** | **str** | Site admin username | [optional] 
**password** | **str** | Site admin password | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.installation_admin_settings_request import InstallationAdminSettingsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationAdminSettingsRequest from a JSON string
installation_admin_settings_request_instance = InstallationAdminSettingsRequest.from_json(json)
# print the JSON string representation of the object
print(InstallationAdminSettingsRequest.to_json())

# convert the object into a dict
installation_admin_settings_request_dict = installation_admin_settings_request_instance.to_dict()
# create an instance of InstallationAdminSettingsRequest from a dict
installation_admin_settings_request_from_dict = InstallationAdminSettingsRequest.from_dict(installation_admin_settings_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


