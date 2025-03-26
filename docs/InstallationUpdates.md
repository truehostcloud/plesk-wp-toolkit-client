# InstallationUpdates


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**applicable** | **bool** | Updates might be disabled by the server administrator | 
**auto_updates_available** | **bool** | Autoupdates availability status | 
**available_version** | **str** | Version of available update | 
**amount_of_plugins_with_updates** | **int** | Number of plugins with available updates | 
**amount_of_themes_with_updates** | **int** | Number of themes with available updates | 
**smart** | [**InstallationSmartUpdates**](InstallationSmartUpdates.md) |  | 
**php** | [**InstallationSmartPhpUpdates**](InstallationSmartPhpUpdates.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_updates import InstallationUpdates

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationUpdates from a JSON string
installation_updates_instance = InstallationUpdates.from_json(json)
# print the JSON string representation of the object
print(InstallationUpdates.to_json())

# convert the object into a dict
installation_updates_dict = installation_updates_instance.to_dict()
# create an instance of InstallationUpdates from a dict
installation_updates_from_dict = InstallationUpdates.from_dict(installation_updates_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


