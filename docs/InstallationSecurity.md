# InstallationSecurity


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available** | **bool** | Availability of security management feature | 
**applicable** | **bool** | Security measures management might be disabled by the server administrator | 
**status** | [**InstallationSecurityStatusEnum**](InstallationSecurityStatusEnum.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_security import InstallationSecurity

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationSecurity from a JSON string
installation_security_instance = InstallationSecurity.from_json(json)
# print the JSON string representation of the object
print(InstallationSecurity.to_json())

# convert the object into a dict
installation_security_dict = installation_security_instance.to_dict()
# create an instance of InstallationSecurity from a dict
installation_security_from_dict = InstallationSecurity.from_dict(installation_security_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


