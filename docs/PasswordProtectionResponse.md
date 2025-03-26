# PasswordProtectionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available** | **bool** | Availability of password protection feature | 
**status** | **bool** | Status | 
**credentials** | [**PasswordProtectionResponseCredentials**](PasswordProtectionResponseCredentials.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.password_protection_response import PasswordProtectionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PasswordProtectionResponse from a JSON string
password_protection_response_instance = PasswordProtectionResponse.from_json(json)
# print the JSON string representation of the object
print(PasswordProtectionResponse.to_json())

# convert the object into a dict
password_protection_response_dict = password_protection_response_instance.to_dict()
# create an instance of PasswordProtectionResponse from a dict
password_protection_response_from_dict = PasswordProtectionResponse.from_dict(password_protection_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


