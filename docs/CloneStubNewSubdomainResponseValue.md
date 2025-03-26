# CloneStubNewSubdomainResponseValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | [**CloneStubNewSubdomainResponseValueName**](CloneStubNewSubdomainResponseValueName.md) |  | 
**parent_domain** | [**CloneStubNewSubdomainResponseValueParentDomain**](CloneStubNewSubdomainResponseValueParentDomain.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.clone_stub_new_subdomain_response_value import CloneStubNewSubdomainResponseValue

# TODO update the JSON string below
json = "{}"
# create an instance of CloneStubNewSubdomainResponseValue from a JSON string
clone_stub_new_subdomain_response_value_instance = CloneStubNewSubdomainResponseValue.from_json(json)
# print the JSON string representation of the object
print(CloneStubNewSubdomainResponseValue.to_json())

# convert the object into a dict
clone_stub_new_subdomain_response_value_dict = clone_stub_new_subdomain_response_value_instance.to_dict()
# create an instance of CloneStubNewSubdomainResponseValue from a dict
clone_stub_new_subdomain_response_value_from_dict = CloneStubNewSubdomainResponseValue.from_dict(clone_stub_new_subdomain_response_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


