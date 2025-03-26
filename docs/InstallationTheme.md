# InstallationTheme


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**slug** | **str** | Theme slug | 
**title** | **str** | Theme title | 
**description** | **str** | Theme description | 
**version** | **str** | Current theme version | 
**available_version** | **str** | Theme version available for update | 
**status** | **bool** | Theme status (active or not) | 
**auto_updates** | **bool** | Theme autoupdate status | 
**auto_updates_available** | **bool** | Theme autoupdate management available | 
**vulnerable** | **bool** | Theme vulnerability status | 
**change_log_url** | **str** | Changelog URL (if update is available) | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.installation_theme import InstallationTheme

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationTheme from a JSON string
installation_theme_instance = InstallationTheme.from_json(json)
# print the JSON string representation of the object
print(InstallationTheme.to_json())

# convert the object into a dict
installation_theme_dict = installation_theme_instance.to_dict()
# create an instance of InstallationTheme from a dict
installation_theme_from_dict = InstallationTheme.from_dict(installation_theme_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


