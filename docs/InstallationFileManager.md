# InstallationFileManager


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available** | **bool** | Availability of file manager feature | 
**url** | **str** | URL to domain file manager | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_file_manager import InstallationFileManager

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationFileManager from a JSON string
installation_file_manager_instance = InstallationFileManager.from_json(json)
# print the JSON string representation of the object
print(InstallationFileManager.to_json())

# convert the object into a dict
installation_file_manager_dict = installation_file_manager_instance.to_dict()
# create an instance of InstallationFileManager from a dict
installation_file_manager_from_dict = InstallationFileManager.from_dict(installation_file_manager_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


