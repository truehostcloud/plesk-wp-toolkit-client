# PasswordProtectionResponseCredentials


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**username** | **str** |  | 
**password** | **str** |  | 

## Example

```python
from plesk_wp_toolkit_client.models.password_protection_response_credentials import PasswordProtectionResponseCredentials

# TODO update the JSON string below
json = "{}"
# create an instance of PasswordProtectionResponseCredentials from a JSON string
password_protection_response_credentials_instance = PasswordProtectionResponseCredentials.from_json(json)
# print the JSON string representation of the object
print(PasswordProtectionResponseCredentials.to_json())

# convert the object into a dict
password_protection_response_credentials_dict = password_protection_response_credentials_instance.to_dict()
# create an instance of PasswordProtectionResponseCredentials from a dict
password_protection_response_credentials_from_dict = PasswordProtectionResponseCredentials.from_dict(password_protection_response_credentials_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


