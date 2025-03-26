# CloneStubMessagesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**multisite_on_subdomains_unix** | [**CloneStubMessagesResponseMultisiteOnSubdomainsUnix**](CloneStubMessagesResponseMultisiteOnSubdomainsUnix.md) |  | [optional] 
**multisite_on_subdomains_windows** | [**CloneStubMessagesResponseMultisiteOnSubdomainsWindows**](CloneStubMessagesResponseMultisiteOnSubdomainsWindows.md) |  | [optional] 
**multisite_on_subdirectories_windows** | [**CloneStubMessagesResponseMultisiteOnSubdirectoriesWindows**](CloneStubMessagesResponseMultisiteOnSubdirectoriesWindows.md) |  | [optional] 
**unable_to_check_database** | [**CloneStubMessagesResponseUnableToCheckDatabase**](CloneStubMessagesResponseUnableToCheckDatabase.md) |  | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.clone_stub_messages_response import CloneStubMessagesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CloneStubMessagesResponse from a JSON string
clone_stub_messages_response_instance = CloneStubMessagesResponse.from_json(json)
# print the JSON string representation of the object
print(CloneStubMessagesResponse.to_json())

# convert the object into a dict
clone_stub_messages_response_dict = clone_stub_messages_response_instance.to_dict()
# create an instance of CloneStubMessagesResponse from a dict
clone_stub_messages_response_from_dict = CloneStubMessagesResponse.from_dict(clone_stub_messages_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


