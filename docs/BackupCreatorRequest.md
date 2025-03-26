# BackupCreatorRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**installation_id** | **int** |  | 
**description** | **str** |  | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.backup_creator_request import BackupCreatorRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BackupCreatorRequest from a JSON string
backup_creator_request_instance = BackupCreatorRequest.from_json(json)
# print the JSON string representation of the object
print(BackupCreatorRequest.to_json())

# convert the object into a dict
backup_creator_request_dict = backup_creator_request_instance.to_dict()
# create an instance of BackupCreatorRequest from a dict
backup_creator_request_from_dict = BackupCreatorRequest.from_dict(backup_creator_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


