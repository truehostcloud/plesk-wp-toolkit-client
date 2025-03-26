# SecurityMeasuresCheckSecurityRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**installations_ids** | **List[int]** |  | 
**skip_broken_installations** | **bool** | Ignore broken installations (by default request fails on them) | [optional] 
**skip_infected_installations** | **bool** | Ignore quarantined installations (by default request fails on them) | [optional] 
**skip_unsupported_installations** | **bool** | Ignore unsupported installations (by default request fails on them) | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.security_measures_check_security_request import SecurityMeasuresCheckSecurityRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SecurityMeasuresCheckSecurityRequest from a JSON string
security_measures_check_security_request_instance = SecurityMeasuresCheckSecurityRequest.from_json(json)
# print the JSON string representation of the object
print(SecurityMeasuresCheckSecurityRequest.to_json())

# convert the object into a dict
security_measures_check_security_request_dict = security_measures_check_security_request_instance.to_dict()
# create an instance of SecurityMeasuresCheckSecurityRequest from a dict
security_measures_check_security_request_from_dict = SecurityMeasuresCheckSecurityRequest.from_dict(security_measures_check_security_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


