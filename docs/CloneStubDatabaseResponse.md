# CloneStubDatabaseResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | [**CloneStubDatabaseResponseValue**](CloneStubDatabaseResponseValue.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.clone_stub_database_response import CloneStubDatabaseResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CloneStubDatabaseResponse from a JSON string
clone_stub_database_response_instance = CloneStubDatabaseResponse.from_json(json)
# print the JSON string representation of the object
print(CloneStubDatabaseResponse.to_json())

# convert the object into a dict
clone_stub_database_response_dict = clone_stub_database_response_instance.to_dict()
# create an instance of CloneStubDatabaseResponse from a dict
clone_stub_database_response_from_dict = CloneStubDatabaseResponse.from_dict(clone_stub_database_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


