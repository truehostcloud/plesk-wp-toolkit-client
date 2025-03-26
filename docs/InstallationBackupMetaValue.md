# InstallationBackupMetaValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_name** | [**InstallationBackupMetaValueFileName**](InstallationBackupMetaValueFileName.md) |  | 
**file_size** | [**InstallationBackupMetaValueFileSize**](InstallationBackupMetaValueFileSize.md) |  | 
**created_at** | [**InstallationBackupMetaValueCreatedAt**](InstallationBackupMetaValueCreatedAt.md) |  | 
**absolute_file_path** | [**InstallationBackupMetaValueAbsoluteFilePath**](InstallationBackupMetaValueAbsoluteFilePath.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_backup_meta_value import InstallationBackupMetaValue

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationBackupMetaValue from a JSON string
installation_backup_meta_value_instance = InstallationBackupMetaValue.from_json(json)
# print the JSON string representation of the object
print(InstallationBackupMetaValue.to_json())

# convert the object into a dict
installation_backup_meta_value_dict = installation_backup_meta_value_instance.to_dict()
# create an instance of InstallationBackupMetaValue from a dict
installation_backup_meta_value_from_dict = InstallationBackupMetaValue.from_dict(installation_backup_meta_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


