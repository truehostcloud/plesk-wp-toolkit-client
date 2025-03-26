# InstallationBackupsMetaResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | [**List[InstallationBackupMeta]**](InstallationBackupMeta.md) | Backups list | 
**meta** | [**InstallationBackupsMetaResponseMeta**](InstallationBackupsMetaResponseMeta.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_backups_meta_response import InstallationBackupsMetaResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationBackupsMetaResponse from a JSON string
installation_backups_meta_response_instance = InstallationBackupsMetaResponse.from_json(json)
# print the JSON string representation of the object
print(InstallationBackupsMetaResponse.to_json())

# convert the object into a dict
installation_backups_meta_response_dict = installation_backups_meta_response_instance.to_dict()
# create an instance of InstallationBackupsMetaResponse from a dict
installation_backups_meta_response_from_dict = InstallationBackupsMetaResponse.from_dict(installation_backups_meta_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


