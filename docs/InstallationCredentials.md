# InstallationCredentials


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available** | **bool** | Availability of login to WordPress feature | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_credentials import InstallationCredentials

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationCredentials from a JSON string
installation_credentials_instance = InstallationCredentials.from_json(json)
# print the JSON string representation of the object
print(InstallationCredentials.to_json())

# convert the object into a dict
installation_credentials_dict = installation_credentials_instance.to_dict()
# create an instance of InstallationCredentials from a dict
installation_credentials_from_dict = InstallationCredentials.from_dict(installation_credentials_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


