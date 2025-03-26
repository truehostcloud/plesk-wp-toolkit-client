# CloneStubInstallationPathResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **str** | Installation path of cloned WordPress site (relative to the root directory of the domain) | 

## Example

```python
from plesk_wp_toolkit_client.models.clone_stub_installation_path_response import CloneStubInstallationPathResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CloneStubInstallationPathResponse from a JSON string
clone_stub_installation_path_response_instance = CloneStubInstallationPathResponse.from_json(json)
# print the JSON string representation of the object
print(CloneStubInstallationPathResponse.to_json())

# convert the object into a dict
clone_stub_installation_path_response_dict = clone_stub_installation_path_response_instance.to_dict()
# create an instance of CloneStubInstallationPathResponse from a dict
clone_stub_installation_path_response_from_dict = CloneStubInstallationPathResponse.from_dict(clone_stub_installation_path_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


