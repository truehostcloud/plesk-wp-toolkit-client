# InstallationDatabaseSettingsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Database name | [optional] 
**server** | **str** | Database server ID (Plesk only) | [optional] 
**user_name** | **str** | Database user name | [optional] 
**user_password** | **str** | Database user password | [optional] 
**table_prefix** | **str** | Database table prefix | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.installation_database_settings_request import InstallationDatabaseSettingsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationDatabaseSettingsRequest from a JSON string
installation_database_settings_request_instance = InstallationDatabaseSettingsRequest.from_json(json)
# print the JSON string representation of the object
print(InstallationDatabaseSettingsRequest.to_json())

# convert the object into a dict
installation_database_settings_request_dict = installation_database_settings_request_instance.to_dict()
# create an instance of InstallationDatabaseSettingsRequest from a dict
installation_database_settings_request_from_dict = InstallationDatabaseSettingsRequest.from_dict(installation_database_settings_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


