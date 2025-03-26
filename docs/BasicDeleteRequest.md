# BasicDeleteRequest

Basic delete request

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**delete** | **bool** | To protect against CSRF attacks the WPT API requires header Content-Type: application/json for request POST/PUT/PATCH/DELETE. On front-end side we use axios, and it automatically removes the Content-Type header for requests when the body is not set. This BasicDeleteRequest is used for all DELETE requests to workaround this, and the BasicConfirmationRequest is used for POST requests (e.g. apply SU results and SU PHP results). | 

## Example

```python
from plesk_wp_toolkit_client.models.basic_delete_request import BasicDeleteRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BasicDeleteRequest from a JSON string
basic_delete_request_instance = BasicDeleteRequest.from_json(json)
# print the JSON string representation of the object
print(BasicDeleteRequest.to_json())

# convert the object into a dict
basic_delete_request_dict = basic_delete_request_instance.to_dict()
# create an instance of BasicDeleteRequest from a dict
basic_delete_request_from_dict = BasicDeleteRequest.from_dict(basic_delete_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


