# MaintenanceTextsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **str** | Browser page title | 
**header** | **str** | Text block 1 (bigger font) | 
**subheader** | **str** | Text block 2 (smaller font) | 

## Example

```python
from plesk_wp_toolkit_client.models.maintenance_texts_request import MaintenanceTextsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of MaintenanceTextsRequest from a JSON string
maintenance_texts_request_instance = MaintenanceTextsRequest.from_json(json)
# print the JSON string representation of the object
print(MaintenanceTextsRequest.to_json())

# convert the object into a dict
maintenance_texts_request_dict = maintenance_texts_request_instance.to_dict()
# create an instance of MaintenanceTextsRequest from a dict
maintenance_texts_request_from_dict = MaintenanceTextsRequest.from_dict(maintenance_texts_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


