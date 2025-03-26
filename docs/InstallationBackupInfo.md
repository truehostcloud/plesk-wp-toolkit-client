# InstallationBackupInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_name** | **str** | Backup file name | 
**file_size** | **float** | Backup file size | 
**created_at** | **str** | Date of backup creation | 
**absolute_file_path** | **str** | Archive absolute file path | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_backup_info import InstallationBackupInfo

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationBackupInfo from a JSON string
installation_backup_info_instance = InstallationBackupInfo.from_json(json)
# print the JSON string representation of the object
print(InstallationBackupInfo.to_json())

# convert the object into a dict
installation_backup_info_dict = installation_backup_info_instance.to_dict()
# create an instance of InstallationBackupInfo from a dict
installation_backup_info_from_dict = InstallationBackupInfo.from_dict(installation_backup_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


