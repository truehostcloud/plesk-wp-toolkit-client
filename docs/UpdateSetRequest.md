# UpdateSetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **str** | Title | 

## Example

```python
from plesk_wp_toolkit_client.models.update_set_request import UpdateSetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateSetRequest from a JSON string
update_set_request_instance = UpdateSetRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateSetRequest.to_json())

# convert the object into a dict
update_set_request_dict = update_set_request_instance.to_dict()
# create an instance of UpdateSetRequest from a dict
update_set_request_from_dict = UpdateSetRequest.from_dict(update_set_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


