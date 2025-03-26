# RefreshAvailableUpdatesRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**installations_ids** | **List[int]** |  | 
**skip_broken_installations** | **bool** | Ignore broken installations (by default request fails on them) | [optional] 
**skip_infected_installations** | **bool** | Ignore quarantined installations (by default request fails on them) | [optional] 
**skip_unsupported_installations** | **bool** | Ignore unsupported installations (by default request fails on them) | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.refresh_available_updates_request import RefreshAvailableUpdatesRequest

# TODO update the JSON string below
json = "{}"
# create an instance of RefreshAvailableUpdatesRequest from a JSON string
refresh_available_updates_request_instance = RefreshAvailableUpdatesRequest.from_json(json)
# print the JSON string representation of the object
print(RefreshAvailableUpdatesRequest.to_json())

# convert the object into a dict
refresh_available_updates_request_dict = refresh_available_updates_request_instance.to_dict()
# create an instance of RefreshAvailableUpdatesRequest from a dict
refresh_available_updates_request_from_dict = RefreshAvailableUpdatesRequest.from_dict(refresh_available_updates_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


