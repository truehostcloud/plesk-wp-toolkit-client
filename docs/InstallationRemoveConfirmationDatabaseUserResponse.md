# InstallationRemoveConfirmationDatabaseUserResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Database user name | 
**shared_with_installations_ids** | **List[int]** | IDs of installations that share database users | 
**removing_allowed** | **bool** | Database user removal allowed during application removal | 
**will_be_removed_automatically** | **bool** | Automatic removal of database user together with application | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_remove_confirmation_database_user_response import InstallationRemoveConfirmationDatabaseUserResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationRemoveConfirmationDatabaseUserResponse from a JSON string
installation_remove_confirmation_database_user_response_instance = InstallationRemoveConfirmationDatabaseUserResponse.from_json(json)
# print the JSON string representation of the object
print(InstallationRemoveConfirmationDatabaseUserResponse.to_json())

# convert the object into a dict
installation_remove_confirmation_database_user_response_dict = installation_remove_confirmation_database_user_response_instance.to_dict()
# create an instance of InstallationRemoveConfirmationDatabaseUserResponse from a dict
installation_remove_confirmation_database_user_response_from_dict = InstallationRemoveConfirmationDatabaseUserResponse.from_dict(installation_remove_confirmation_database_user_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


