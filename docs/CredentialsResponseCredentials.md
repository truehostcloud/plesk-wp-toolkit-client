# CredentialsResponseCredentials


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**login** | **str** | WordPress admin dashboard username | 
**password** | **str** | WordPress admin dashboard password | 

## Example

```python
from plesk_wp_toolkit_client.models.credentials_response_credentials import CredentialsResponseCredentials

# TODO update the JSON string below
json = "{}"
# create an instance of CredentialsResponseCredentials from a JSON string
credentials_response_credentials_instance = CredentialsResponseCredentials.from_json(json)
# print the JSON string representation of the object
print(CredentialsResponseCredentials.to_json())

# convert the object into a dict
credentials_response_credentials_dict = credentials_response_credentials_instance.to_dict()
# create an instance of CredentialsResponseCredentials from a dict
credentials_response_credentials_from_dict = CredentialsResponseCredentials.from_dict(credentials_response_credentials_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


