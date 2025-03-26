# InstallationRestorePoint


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available** | **bool** | Restore point creation availability | 
**restore_point_timestamp** | **int** | Restore point timestamp | 
**previous_version** | **str** | Source version of WordPress | 
**version** | **str** | Target version of WordPress | 
**error_message** | **str** | Error message | 
**display_timestamp** | **str** | Localized timestamp | 
**full_snapshot** | **bool** | Snapshot scope (full or partial) | 
**message** | **str** | Tooltip message for UI | 
**source_url** | **str** | Source WordPress URL | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_restore_point import InstallationRestorePoint

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationRestorePoint from a JSON string
installation_restore_point_instance = InstallationRestorePoint.from_json(json)
# print the JSON string representation of the object
print(InstallationRestorePoint.to_json())

# convert the object into a dict
installation_restore_point_dict = installation_restore_point_instance.to_dict()
# create an instance of InstallationRestorePoint from a dict
installation_restore_point_from_dict = InstallationRestorePoint.from_dict(installation_restore_point_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


