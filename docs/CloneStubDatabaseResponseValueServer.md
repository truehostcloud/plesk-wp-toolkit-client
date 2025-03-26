# CloneStubDatabaseResponseValueServer


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **str** | Database server ID (Plesk only) | 
**meta** | [**CloneStubDatabaseResponseValueServerMeta**](CloneStubDatabaseResponseValueServerMeta.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.clone_stub_database_response_value_server import CloneStubDatabaseResponseValueServer

# TODO update the JSON string below
json = "{}"
# create an instance of CloneStubDatabaseResponseValueServer from a JSON string
clone_stub_database_response_value_server_instance = CloneStubDatabaseResponseValueServer.from_json(json)
# print the JSON string representation of the object
print(CloneStubDatabaseResponseValueServer.to_json())

# convert the object into a dict
clone_stub_database_response_value_server_dict = clone_stub_database_response_value_server_instance.to_dict()
# create an instance of CloneStubDatabaseResponseValueServer from a dict
clone_stub_database_response_value_server_from_dict = CloneStubDatabaseResponseValueServer.from_dict(clone_stub_database_response_value_server_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


