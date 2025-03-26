# Integrity


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available** | **bool** | Availability of &#39;Check WordPress Integrity&#39; feature | 
**tasks** | [**IntegrityTasks**](IntegrityTasks.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.integrity import Integrity

# TODO update the JSON string below
json = "{}"
# create an instance of Integrity from a JSON string
integrity_instance = Integrity.from_json(json)
# print the JSON string representation of the object
print(Integrity.to_json())

# convert the object into a dict
integrity_dict = integrity_instance.to_dict()
# create an instance of Integrity from a dict
integrity_from_dict = Integrity.from_dict(integrity_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


