# PasswordProtectionRequestCredentials


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**username** | **str** |  | 
**password** | **str** |  | 

## Example

```python
from plesk_wp_toolkit_client.models.password_protection_request_credentials import PasswordProtectionRequestCredentials

# TODO update the JSON string below
json = "{}"
# create an instance of PasswordProtectionRequestCredentials from a JSON string
password_protection_request_credentials_instance = PasswordProtectionRequestCredentials.from_json(json)
# print the JSON string representation of the object
print(PasswordProtectionRequestCredentials.to_json())

# convert the object into a dict
password_protection_request_credentials_dict = password_protection_request_credentials_instance.to_dict()
# create an instance of PasswordProtectionRequestCredentials from a dict
password_protection_request_credentials_from_dict = PasswordProtectionRequestCredentials.from_dict(password_protection_request_credentials_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


