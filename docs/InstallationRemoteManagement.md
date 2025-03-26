# InstallationRemoteManagement


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available** | **bool** | Availability of remote management feature | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_remote_management import InstallationRemoteManagement

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationRemoteManagement from a JSON string
installation_remote_management_instance = InstallationRemoteManagement.from_json(json)
# print the JSON string representation of the object
print(InstallationRemoteManagement.to_json())

# convert the object into a dict
installation_remote_management_dict = installation_remote_management_instance.to_dict()
# create an instance of InstallationRemoteManagement from a dict
installation_remote_management_from_dict = InstallationRemoteManagement.from_dict(installation_remote_management_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


