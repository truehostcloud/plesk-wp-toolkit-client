# InstallationPlugin


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**slug** | **str** | Plugin slug | 
**title** | **str** | Plugin title | 
**description** | **str** | Plugin description | 
**version** | **str** | Current plugin version | 
**available_version** | **str** | Plugin version available for update | 
**status** | **bool** | Plugin status (active or not) | 
**must_use** | **bool** | Plugin is must-use (if true) | 
**auto_updates** | **bool** | Plugin autoupdate status | 
**auto_updates_available** | **bool** | Plugin autoupdate management available | 
**vulnerable** | **bool** | Plugin vulnerability status | 
**change_log_url** | **str** | Changelog URL (if update is available) | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.installation_plugin import InstallationPlugin

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationPlugin from a JSON string
installation_plugin_instance = InstallationPlugin.from_json(json)
# print the JSON string representation of the object
print(InstallationPlugin.to_json())

# convert the object into a dict
installation_plugin_dict = installation_plugin_instance.to_dict()
# create an instance of InstallationPlugin from a dict
installation_plugin_from_dict = InstallationPlugin.from_dict(installation_plugin_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


