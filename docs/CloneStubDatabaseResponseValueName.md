# CloneStubDatabaseResponseValueName


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **str** | Database name | 
**meta** | [**CloneStubDatabaseResponseValueNameMeta**](CloneStubDatabaseResponseValueNameMeta.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.clone_stub_database_response_value_name import CloneStubDatabaseResponseValueName

# TODO update the JSON string below
json = "{}"
# create an instance of CloneStubDatabaseResponseValueName from a JSON string
clone_stub_database_response_value_name_instance = CloneStubDatabaseResponseValueName.from_json(json)
# print the JSON string representation of the object
print(CloneStubDatabaseResponseValueName.to_json())

# convert the object into a dict
clone_stub_database_response_value_name_dict = clone_stub_database_response_value_name_instance.to_dict()
# create an instance of CloneStubDatabaseResponseValueName from a dict
clone_stub_database_response_value_name_from_dict = CloneStubDatabaseResponseValueName.from_dict(clone_stub_database_response_value_name_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


