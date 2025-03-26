# InstallationPasswordProtection


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available** | **bool** | Availability of password protection feature | 
**status** | **bool** | Password protection feature status | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_password_protection import InstallationPasswordProtection

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationPasswordProtection from a JSON string
installation_password_protection_instance = InstallationPasswordProtection.from_json(json)
# print the JSON string representation of the object
print(InstallationPasswordProtection.to_json())

# convert the object into a dict
installation_password_protection_dict = installation_password_protection_instance.to_dict()
# create an instance of InstallationPasswordProtection from a dict
installation_password_protection_from_dict = InstallationPasswordProtection.from_dict(installation_password_protection_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


