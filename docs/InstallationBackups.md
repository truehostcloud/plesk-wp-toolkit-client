# InstallationBackups


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**panel_backups_available** | **bool** | Availability of panel backup feature | 
**wpt_backups_available** | **bool** | Availability of WP Toolkit backup feature | 
**backup_manager_url** | **str** | URL to domain backup manager | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_backups import InstallationBackups

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationBackups from a JSON string
installation_backups_instance = InstallationBackups.from_json(json)
# print the JSON string representation of the object
print(InstallationBackups.to_json())

# convert the object into a dict
installation_backups_dict = installation_backups_instance.to_dict()
# create an instance of InstallationBackups from a dict
installation_backups_from_dict = InstallationBackups.from_dict(installation_backups_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


