# InstallationSmartPhpUpdates


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available** | **bool** | Availability of Smart PHP Update feature | 
**applicable** | **bool** | Smart PHP Update might be disabled by the server administrator | 
**task_status** | [**InstallationSmartPhpUpdatesTaskStatusEnum**](InstallationSmartPhpUpdatesTaskStatusEnum.md) |  | 
**created_at** | **datetime** | Date and time when Smart PHP Update result was created | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_smart_php_updates import InstallationSmartPhpUpdates

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationSmartPhpUpdates from a JSON string
installation_smart_php_updates_instance = InstallationSmartPhpUpdates.from_json(json)
# print the JSON string representation of the object
print(InstallationSmartPhpUpdates.to_json())

# convert the object into a dict
installation_smart_php_updates_dict = installation_smart_php_updates_instance.to_dict()
# create an instance of InstallationSmartPhpUpdates from a dict
installation_smart_php_updates_from_dict = InstallationSmartPhpUpdates.from_dict(installation_smart_php_updates_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


