# InstallationBackupMeta


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | **object** |  | 
**value** | [**InstallationBackupMetaValue**](InstallationBackupMetaValue.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_backup_meta import InstallationBackupMeta

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationBackupMeta from a JSON string
installation_backup_meta_instance = InstallationBackupMeta.from_json(json)
# print the JSON string representation of the object
print(InstallationBackupMeta.to_json())

# convert the object into a dict
installation_backup_meta_dict = installation_backup_meta_instance.to_dict()
# create an instance of InstallationBackupMeta from a dict
installation_backup_meta_from_dict = InstallationBackupMeta.from_dict(installation_backup_meta_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


