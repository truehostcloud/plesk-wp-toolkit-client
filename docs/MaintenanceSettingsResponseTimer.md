# MaintenanceSettingsResponseTimer

Countdown timer

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** | Enable timer | 
**days** | **float** | Remaining days | 
**hours** | **float** | Remaining hours | 
**minutes** | **float** | Remaining minutes | 

## Example

```python
from plesk_wp_toolkit_client.models.maintenance_settings_response_timer import MaintenanceSettingsResponseTimer

# TODO update the JSON string below
json = "{}"
# create an instance of MaintenanceSettingsResponseTimer from a JSON string
maintenance_settings_response_timer_instance = MaintenanceSettingsResponseTimer.from_json(json)
# print the JSON string representation of the object
print(MaintenanceSettingsResponseTimer.to_json())

# convert the object into a dict
maintenance_settings_response_timer_dict = maintenance_settings_response_timer_instance.to_dict()
# create an instance of MaintenanceSettingsResponseTimer from a dict
maintenance_settings_response_timer_from_dict = MaintenanceSettingsResponseTimer.from_dict(maintenance_settings_response_timer_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


