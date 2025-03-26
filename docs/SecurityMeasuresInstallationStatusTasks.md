# SecurityMeasuresInstallationStatusTasks


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**check** | [**BackgroundTaskResponse**](BackgroundTaskResponse.md) |  | 
**resolve** | [**BackgroundTaskResponse**](BackgroundTaskResponse.md) |  | 
**revert** | [**BackgroundTaskResponse**](BackgroundTaskResponse.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.security_measures_installation_status_tasks import SecurityMeasuresInstallationStatusTasks

# TODO update the JSON string below
json = "{}"
# create an instance of SecurityMeasuresInstallationStatusTasks from a JSON string
security_measures_installation_status_tasks_instance = SecurityMeasuresInstallationStatusTasks.from_json(json)
# print the JSON string representation of the object
print(SecurityMeasuresInstallationStatusTasks.to_json())

# convert the object into a dict
security_measures_installation_status_tasks_dict = security_measures_installation_status_tasks_instance.to_dict()
# create an instance of SecurityMeasuresInstallationStatusTasks from a dict
security_measures_installation_status_tasks_from_dict = SecurityMeasuresInstallationStatusTasks.from_dict(security_measures_installation_status_tasks_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


