# CloneStubDomainResponseValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**existing** | [**CloneStubDomainResponseValueExisting**](CloneStubDomainResponseValueExisting.md) |  | 
**new_subdomain** | [**CloneStubNewSubdomainResponse**](CloneStubNewSubdomainResponse.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.clone_stub_domain_response_value import CloneStubDomainResponseValue

# TODO update the JSON string below
json = "{}"
# create an instance of CloneStubDomainResponseValue from a JSON string
clone_stub_domain_response_value_instance = CloneStubDomainResponseValue.from_json(json)
# print the JSON string representation of the object
print(CloneStubDomainResponseValue.to_json())

# convert the object into a dict
clone_stub_domain_response_value_dict = clone_stub_domain_response_value_instance.to_dict()
# create an instance of CloneStubDomainResponseValue from a dict
clone_stub_domain_response_value_from_dict = CloneStubDomainResponseValue.from_dict(clone_stub_domain_response_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


