# InstallationRemoveConfirmationResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Installation ID | 
**database** | [**InstallationRemoveConfirmationDatabaseResponse**](InstallationRemoveConfirmationDatabaseResponse.md) |  | 
**user** | [**InstallationRemoveConfirmationDatabaseUserResponse**](InstallationRemoveConfirmationDatabaseUserResponse.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_remove_confirmation_response import InstallationRemoveConfirmationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationRemoveConfirmationResponse from a JSON string
installation_remove_confirmation_response_instance = InstallationRemoveConfirmationResponse.from_json(json)
# print the JSON string representation of the object
print(InstallationRemoveConfirmationResponse.to_json())

# convert the object into a dict
installation_remove_confirmation_response_dict = installation_remove_confirmation_response_instance.to_dict()
# create an instance of InstallationRemoveConfirmationResponse from a dict
installation_remove_confirmation_response_from_dict = InstallationRemoveConfirmationResponse.from_dict(installation_remove_confirmation_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


