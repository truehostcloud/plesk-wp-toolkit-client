# SecurityMeasure


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**title** | **str** |  | 
**description** | **str** |  | 
**rollback_available** | **bool** | Ability to revert this security measure | 
**critical** | **bool** | WP Toolkit recommends to apply all critical security measures | 

## Example

```python
from plesk_wp_toolkit_client.models.security_measure import SecurityMeasure

# TODO update the JSON string below
json = "{}"
# create an instance of SecurityMeasure from a JSON string
security_measure_instance = SecurityMeasure.from_json(json)
# print the JSON string representation of the object
print(SecurityMeasure.to_json())

# convert the object into a dict
security_measure_dict = security_measure_instance.to_dict()
# create an instance of SecurityMeasure from a dict
security_measure_from_dict = SecurityMeasure.from_dict(security_measure_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


