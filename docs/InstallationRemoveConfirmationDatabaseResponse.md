# InstallationRemoveConfirmationDatabaseResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Database name | 
**shared_with_installations_ids** | **List[int]** | IDs of installations that share databases | 
**removing_allowed** | **bool** | Database removal allowed during application removal | 
**will_be_removed_automatically** | **bool** | Automatic removal of database together with application | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_remove_confirmation_database_response import InstallationRemoveConfirmationDatabaseResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationRemoveConfirmationDatabaseResponse from a JSON string
installation_remove_confirmation_database_response_instance = InstallationRemoveConfirmationDatabaseResponse.from_json(json)
# print the JSON string representation of the object
print(InstallationRemoveConfirmationDatabaseResponse.to_json())

# convert the object into a dict
installation_remove_confirmation_database_response_dict = installation_remove_confirmation_database_response_instance.to_dict()
# create an instance of InstallationRemoveConfirmationDatabaseResponse from a dict
installation_remove_confirmation_database_response_from_dict = InstallationRemoveConfirmationDatabaseResponse.from_dict(installation_remove_confirmation_database_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


