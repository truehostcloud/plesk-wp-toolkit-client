# CloneStubNewSubdomainResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | [**CloneStubNewSubdomainResponseValue**](CloneStubNewSubdomainResponseValue.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.clone_stub_new_subdomain_response import CloneStubNewSubdomainResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CloneStubNewSubdomainResponse from a JSON string
clone_stub_new_subdomain_response_instance = CloneStubNewSubdomainResponse.from_json(json)
# print the JSON string representation of the object
print(CloneStubNewSubdomainResponse.to_json())

# convert the object into a dict
clone_stub_new_subdomain_response_dict = clone_stub_new_subdomain_response_instance.to_dict()
# create an instance of CloneStubNewSubdomainResponse from a dict
clone_stub_new_subdomain_response_from_dict = CloneStubNewSubdomainResponse.from_dict(clone_stub_new_subdomain_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


