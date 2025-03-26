# CloneStubDomainResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | [**CloneStubDomainResponseValue**](CloneStubDomainResponseValue.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.clone_stub_domain_response import CloneStubDomainResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CloneStubDomainResponse from a JSON string
clone_stub_domain_response_instance = CloneStubDomainResponse.from_json(json)
# print the JSON string representation of the object
print(CloneStubDomainResponse.to_json())

# convert the object into a dict
clone_stub_domain_response_dict = clone_stub_domain_response_instance.to_dict()
# create an instance of CloneStubDomainResponse from a dict
clone_stub_domain_response_from_dict = CloneStubDomainResponse.from_dict(clone_stub_domain_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


