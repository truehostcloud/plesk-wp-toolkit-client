# InstallationMultipleSitesManagement


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**applicable** | **bool** | Availability of mass site management feature | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_multiple_sites_management import InstallationMultipleSitesManagement

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationMultipleSitesManagement from a JSON string
installation_multiple_sites_management_instance = InstallationMultipleSitesManagement.from_json(json)
# print the JSON string representation of the object
print(InstallationMultipleSitesManagement.to_json())

# convert the object into a dict
installation_multiple_sites_management_dict = installation_multiple_sites_management_instance.to_dict()
# create an instance of InstallationMultipleSitesManagement from a dict
installation_multiple_sites_management_from_dict = InstallationMultipleSitesManagement.from_dict(installation_multiple_sites_management_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


