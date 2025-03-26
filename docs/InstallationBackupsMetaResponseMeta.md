# InstallationBackupsMetaResponseMeta


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**limit** | **int** | Service plan limit of installation backups | 
**file_manager_url** | **str** | File Manager URL for backups directory | 
**dir_name** | **str** | Backups directory name | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_backups_meta_response_meta import InstallationBackupsMetaResponseMeta

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationBackupsMetaResponseMeta from a JSON string
installation_backups_meta_response_meta_instance = InstallationBackupsMetaResponseMeta.from_json(json)
# print the JSON string representation of the object
print(InstallationBackupsMetaResponseMeta.to_json())

# convert the object into a dict
installation_backups_meta_response_meta_dict = installation_backups_meta_response_meta_instance.to_dict()
# create an instance of InstallationBackupsMetaResponseMeta from a dict
installation_backups_meta_response_meta_from_dict = InstallationBackupsMetaResponseMeta.from_dict(installation_backups_meta_response_meta_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


