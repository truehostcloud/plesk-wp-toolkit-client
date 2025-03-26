# SmartUpdateCloneInstallation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Installation ID of target WordPress site | 
**url** | **str** | URL of target WordPress site | 

## Example

```python
from plesk_wp_toolkit_client.models.smart_update_clone_installation import SmartUpdateCloneInstallation

# TODO update the JSON string below
json = "{}"
# create an instance of SmartUpdateCloneInstallation from a JSON string
smart_update_clone_installation_instance = SmartUpdateCloneInstallation.from_json(json)
# print the JSON string representation of the object
print(SmartUpdateCloneInstallation.to_json())

# convert the object into a dict
smart_update_clone_installation_dict = smart_update_clone_installation_instance.to_dict()
# create an instance of SmartUpdateCloneInstallation from a dict
smart_update_clone_installation_from_dict = SmartUpdateCloneInstallation.from_dict(smart_update_clone_installation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


