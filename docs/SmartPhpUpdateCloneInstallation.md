# SmartPhpUpdateCloneInstallation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Installation ID of target WordPress site | 
**url** | **str** | URL of target WordPress site | 

## Example

```python
from plesk_wp_toolkit_client.models.smart_php_update_clone_installation import SmartPhpUpdateCloneInstallation

# TODO update the JSON string below
json = "{}"
# create an instance of SmartPhpUpdateCloneInstallation from a JSON string
smart_php_update_clone_installation_instance = SmartPhpUpdateCloneInstallation.from_json(json)
# print the JSON string representation of the object
print(SmartPhpUpdateCloneInstallation.to_json())

# convert the object into a dict
smart_php_update_clone_installation_dict = smart_php_update_clone_installation_instance.to_dict()
# create an instance of SmartPhpUpdateCloneInstallation from a dict
smart_php_update_clone_installation_from_dict = SmartPhpUpdateCloneInstallation.from_dict(smart_php_update_clone_installation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


