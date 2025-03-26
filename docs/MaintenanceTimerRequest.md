# MaintenanceTimerRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** | Enable timer | 
**days** | **float** | Remaining days | 
**hours** | **float** | Remaining hours | 
**minutes** | **float** | Remaining minutes | 

## Example

```python
from plesk_wp_toolkit_client.models.maintenance_timer_request import MaintenanceTimerRequest

# TODO update the JSON string below
json = "{}"
# create an instance of MaintenanceTimerRequest from a JSON string
maintenance_timer_request_instance = MaintenanceTimerRequest.from_json(json)
# print the JSON string representation of the object
print(MaintenanceTimerRequest.to_json())

# convert the object into a dict
maintenance_timer_request_dict = maintenance_timer_request_instance.to_dict()
# create an instance of MaintenanceTimerRequest from a dict
maintenance_timer_request_from_dict = MaintenanceTimerRequest.from_dict(maintenance_timer_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


