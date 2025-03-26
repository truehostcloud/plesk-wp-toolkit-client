# InstallationPluginsBlockList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount_of_blocked_plugins** | **float** | Number of plugins in the blocklist | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_plugins_block_list import InstallationPluginsBlockList

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationPluginsBlockList from a JSON string
installation_plugins_block_list_instance = InstallationPluginsBlockList.from_json(json)
# print the JSON string representation of the object
print(InstallationPluginsBlockList.to_json())

# convert the object into a dict
installation_plugins_block_list_dict = installation_plugins_block_list_instance.to_dict()
# create an instance of InstallationPluginsBlockList from a dict
installation_plugins_block_list_from_dict = InstallationPluginsBlockList.from_dict(installation_plugins_block_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


