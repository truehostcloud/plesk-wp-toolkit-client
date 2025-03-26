# InstallationMaintenance


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **bool** | Maintenance feature status | 
**full_mode** | **bool** | Maintenance mode is fully restricting access to WordPress dashboard | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_maintenance import InstallationMaintenance

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationMaintenance from a JSON string
installation_maintenance_instance = InstallationMaintenance.from_json(json)
# print the JSON string representation of the object
print(InstallationMaintenance.to_json())

# convert the object into a dict
installation_maintenance_dict = installation_maintenance_instance.to_dict()
# create an instance of InstallationMaintenance from a dict
installation_maintenance_from_dict = InstallationMaintenance.from_dict(installation_maintenance_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


