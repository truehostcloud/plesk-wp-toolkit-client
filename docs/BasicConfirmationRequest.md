# BasicConfirmationRequest

Basic confirmation request

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**confirm** | **bool** |  | 

## Example

```python
from plesk_wp_toolkit_client.models.basic_confirmation_request import BasicConfirmationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BasicConfirmationRequest from a JSON string
basic_confirmation_request_instance = BasicConfirmationRequest.from_json(json)
# print the JSON string representation of the object
print(BasicConfirmationRequest.to_json())

# convert the object into a dict
basic_confirmation_request_dict = basic_confirmation_request_instance.to_dict()
# create an instance of BasicConfirmationRequest from a dict
basic_confirmation_request_from_dict = BasicConfirmationRequest.from_dict(basic_confirmation_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


