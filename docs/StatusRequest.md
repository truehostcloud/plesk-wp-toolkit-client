# StatusRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **bool** | Status | 

## Example

```python
from plesk_wp_toolkit_client.models.status_request import StatusRequest

# TODO update the JSON string below
json = "{}"
# create an instance of StatusRequest from a JSON string
status_request_instance = StatusRequest.from_json(json)
# print the JSON string representation of the object
print(StatusRequest.to_json())

# convert the object into a dict
status_request_dict = status_request_instance.to_dict()
# create an instance of StatusRequest from a dict
status_request_from_dict = StatusRequest.from_dict(status_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


