# CloneStubResponseValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**database** | [**CloneStubDatabaseResponse**](CloneStubDatabaseResponse.md) |  | 
**domain** | [**CloneStubDomainResponse**](CloneStubDomainResponse.md) |  | 
**installation_path** | [**CloneStubInstallationPathResponse**](CloneStubInstallationPathResponse.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.clone_stub_response_value import CloneStubResponseValue

# TODO update the JSON string below
json = "{}"
# create an instance of CloneStubResponseValue from a JSON string
clone_stub_response_value_instance = CloneStubResponseValue.from_json(json)
# print the JSON string representation of the object
print(CloneStubResponseValue.to_json())

# convert the object into a dict
clone_stub_response_value_dict = clone_stub_response_value_instance.to_dict()
# create an instance of CloneStubResponseValue from a dict
clone_stub_response_value_from_dict = CloneStubResponseValue.from_dict(clone_stub_response_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


