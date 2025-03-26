# PasswordProtectionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **bool** | Status | [optional] 
**credentials** | [**PasswordProtectionRequestCredentials**](PasswordProtectionRequestCredentials.md) |  | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.password_protection_request import PasswordProtectionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PasswordProtectionRequest from a JSON string
password_protection_request_instance = PasswordProtectionRequest.from_json(json)
# print the JSON string representation of the object
print(PasswordProtectionRequest.to_json())

# convert the object into a dict
password_protection_request_dict = password_protection_request_instance.to_dict()
# create an instance of PasswordProtectionRequest from a dict
password_protection_request_from_dict = PasswordProtectionRequest.from_dict(password_protection_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


