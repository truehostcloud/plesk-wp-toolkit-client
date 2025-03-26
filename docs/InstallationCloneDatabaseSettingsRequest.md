# InstallationCloneDatabaseSettingsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Database name | 
**name_prefix** | **str** | Database name prefix | [optional] 
**server** | **str** | Database server ID (Plesk only) | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.installation_clone_database_settings_request import InstallationCloneDatabaseSettingsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationCloneDatabaseSettingsRequest from a JSON string
installation_clone_database_settings_request_instance = InstallationCloneDatabaseSettingsRequest.from_json(json)
# print the JSON string representation of the object
print(InstallationCloneDatabaseSettingsRequest.to_json())

# convert the object into a dict
installation_clone_database_settings_request_dict = installation_clone_database_settings_request_instance.to_dict()
# create an instance of InstallationCloneDatabaseSettingsRequest from a dict
installation_clone_database_settings_request_from_dict = InstallationCloneDatabaseSettingsRequest.from_dict(installation_clone_database_settings_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


