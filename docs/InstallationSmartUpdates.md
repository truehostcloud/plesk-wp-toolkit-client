# InstallationSmartUpdates


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available** | **bool** | Availability of Smart Update feature | 
**applicable** | **bool** | Smart Updates might be disabled by the server administrator | 
**promo_available** | **bool** | Show Smart Update promo banner | 
**status** | **bool** | Smart Update enabled | 
**task_status** | [**InstallationSmartUpdatesTaskStatusEnum**](InstallationSmartUpdatesTaskStatusEnum.md) |  | 
**initiated_by_auto_updater** | **bool** | Smart Update launched in scope of autoupdate task (might require user attention) | 
**created_at** | **datetime** | Date and time when Smart Update result was created | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_smart_updates import InstallationSmartUpdates

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationSmartUpdates from a JSON string
installation_smart_updates_instance = InstallationSmartUpdates.from_json(json)
# print the JSON string representation of the object
print(InstallationSmartUpdates.to_json())

# convert the object into a dict
installation_smart_updates_dict = installation_smart_updates_instance.to_dict()
# create an instance of InstallationSmartUpdates from a dict
installation_smart_updates_from_dict = InstallationSmartUpdates.from_dict(installation_smart_updates_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


