# SecurityMeasuresResolveRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**installations_ids** | **List[int]** |  | 
**skip_broken_installations** | **bool** | Ignore broken installations (by default request fails on them) | [optional] 
**skip_infected_installations** | **bool** | Ignore quarantined installations (by default request fails on them) | [optional] 
**skip_unsupported_installations** | **bool** | Ignore unsupported installations (by default request fails on them) | [optional] 
**security_measures** | **List[str]** |  | 

## Example

```python
from plesk_wp_toolkit_client.models.security_measures_resolve_request import SecurityMeasuresResolveRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SecurityMeasuresResolveRequest from a JSON string
security_measures_resolve_request_instance = SecurityMeasuresResolveRequest.from_json(json)
# print the JSON string representation of the object
print(SecurityMeasuresResolveRequest.to_json())

# convert the object into a dict
security_measures_resolve_request_dict = security_measures_resolve_request_instance.to_dict()
# create an instance of SecurityMeasuresResolveRequest from a dict
security_measures_resolve_request_from_dict = SecurityMeasuresResolveRequest.from_dict(security_measures_resolve_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


