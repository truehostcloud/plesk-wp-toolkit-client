# CloneStubResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | [**CloneStubResponseValue**](CloneStubResponseValue.md) |  | 
**meta** | [**CloneStubResponseMeta**](CloneStubResponseMeta.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.clone_stub_response import CloneStubResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CloneStubResponse from a JSON string
clone_stub_response_instance = CloneStubResponse.from_json(json)
# print the JSON string representation of the object
print(CloneStubResponse.to_json())

# convert the object into a dict
clone_stub_response_dict = clone_stub_response_instance.to_dict()
# create an instance of CloneStubResponse from a dict
clone_stub_response_from_dict = CloneStubResponse.from_dict(clone_stub_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


