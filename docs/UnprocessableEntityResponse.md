# UnprocessableEntityResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | 
**form_errors** | **object** |  | 

## Example

```python
from plesk_wp_toolkit_client.models.unprocessable_entity_response import UnprocessableEntityResponse

# TODO update the JSON string below
json = "{}"
# create an instance of UnprocessableEntityResponse from a JSON string
unprocessable_entity_response_instance = UnprocessableEntityResponse.from_json(json)
# print the JSON string representation of the object
print(UnprocessableEntityResponse.to_json())

# convert the object into a dict
unprocessable_entity_response_dict = unprocessable_entity_response_instance.to_dict()
# create an instance of UnprocessableEntityResponse from a dict
unprocessable_entity_response_from_dict = UnprocessableEntityResponse.from_dict(unprocessable_entity_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


