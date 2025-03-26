# MaintenanceSocialNetworksRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**facebook** | **str** | Link to Facebook | 
**twitter** | **str** | Link to Twitter | 
**instagram** | **str** | Link to Instagram | 

## Example

```python
from plesk_wp_toolkit_client.models.maintenance_social_networks_request import MaintenanceSocialNetworksRequest

# TODO update the JSON string below
json = "{}"
# create an instance of MaintenanceSocialNetworksRequest from a JSON string
maintenance_social_networks_request_instance = MaintenanceSocialNetworksRequest.from_json(json)
# print the JSON string representation of the object
print(MaintenanceSocialNetworksRequest.to_json())

# convert the object into a dict
maintenance_social_networks_request_dict = maintenance_social_networks_request_instance.to_dict()
# create an instance of MaintenanceSocialNetworksRequest from a dict
maintenance_social_networks_request_from_dict = MaintenanceSocialNetworksRequest.from_dict(maintenance_social_networks_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


