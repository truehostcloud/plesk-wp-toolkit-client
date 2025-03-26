# LaunchInstallationUpdate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**installation_id** | **int** |  | 
**core** | [**CoreUpdateInfo**](CoreUpdateInfo.md) |  | 
**plugins** | **List[str]** | Plugin slugs to update | 
**themes** | **List[str]** | Theme slugs to update | 

## Example

```python
from plesk_wp_toolkit_client.models.launch_installation_update import LaunchInstallationUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of LaunchInstallationUpdate from a JSON string
launch_installation_update_instance = LaunchInstallationUpdate.from_json(json)
# print the JSON string representation of the object
print(LaunchInstallationUpdate.to_json())

# convert the object into a dict
launch_installation_update_dict = launch_installation_update_instance.to_dict()
# create an instance of LaunchInstallationUpdate from a dict
launch_installation_update_from_dict = LaunchInstallationUpdate.from_dict(launch_installation_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


