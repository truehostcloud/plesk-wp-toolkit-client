# InstallationSecurityMeasure


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**status** | **bool** | Activity status of security measure | 
**available** | **bool** | Availability of security measure | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_security_measure import InstallationSecurityMeasure

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationSecurityMeasure from a JSON string
installation_security_measure_instance = InstallationSecurityMeasure.from_json(json)
# print the JSON string representation of the object
print(InstallationSecurityMeasure.to_json())

# convert the object into a dict
installation_security_measure_dict = installation_security_measure_instance.to_dict()
# create an instance of InstallationSecurityMeasure from a dict
installation_security_measure_from_dict = InstallationSecurityMeasure.from_dict(installation_security_measure_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


