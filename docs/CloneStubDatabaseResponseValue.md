# CloneStubDatabaseResponseValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | [**CloneStubDatabaseResponseValueName**](CloneStubDatabaseResponseValueName.md) |  | 
**name_prefix** | [**CloneStubDatabaseResponseValueNamePrefix**](CloneStubDatabaseResponseValueNamePrefix.md) |  | 
**server** | [**CloneStubDatabaseResponseValueServer**](CloneStubDatabaseResponseValueServer.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.clone_stub_database_response_value import CloneStubDatabaseResponseValue

# TODO update the JSON string below
json = "{}"
# create an instance of CloneStubDatabaseResponseValue from a JSON string
clone_stub_database_response_value_instance = CloneStubDatabaseResponseValue.from_json(json)
# print the JSON string representation of the object
print(CloneStubDatabaseResponseValue.to_json())

# convert the object into a dict
clone_stub_database_response_value_dict = clone_stub_database_response_value_instance.to_dict()
# create an instance of CloneStubDatabaseResponseValue from a dict
clone_stub_database_response_value_from_dict = CloneStubDatabaseResponseValue.from_dict(clone_stub_database_response_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


