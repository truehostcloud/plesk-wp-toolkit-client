# BackupRestorerRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**installation_id** | **int** |  | 
**file_name** | **str** |  | 
**clobber** | **bool** | If true files not present in backup will be removed from installation | [optional] 
**drop_all_database_tables** | **bool** |  | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.backup_restorer_request import BackupRestorerRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BackupRestorerRequest from a JSON string
backup_restorer_request_instance = BackupRestorerRequest.from_json(json)
# print the JSON string representation of the object
print(BackupRestorerRequest.to_json())

# convert the object into a dict
backup_restorer_request_dict = backup_restorer_request_instance.to_dict()
# create an instance of BackupRestorerRequest from a dict
backup_restorer_request_from_dict = BackupRestorerRequest.from_dict(backup_restorer_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


