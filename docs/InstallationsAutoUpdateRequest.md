# InstallationsAutoUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**installations_ids** | **List[int]** |  | 
**auto_update** | [**InstallationAutoUpdateRequest**](InstallationAutoUpdateRequest.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.installations_auto_update_request import InstallationsAutoUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationsAutoUpdateRequest from a JSON string
installations_auto_update_request_instance = InstallationsAutoUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(InstallationsAutoUpdateRequest.to_json())

# convert the object into a dict
installations_auto_update_request_dict = installations_auto_update_request_instance.to_dict()
# create an instance of InstallationsAutoUpdateRequest from a dict
installations_auto_update_request_from_dict = InstallationsAutoUpdateRequest.from_dict(installations_auto_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


