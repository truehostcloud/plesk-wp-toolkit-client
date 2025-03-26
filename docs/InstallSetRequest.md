# InstallSetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**set_id** | **int** | Set ID | 
**installation_id** | **int** | Installation ID | 

## Example

```python
from plesk_wp_toolkit_client.models.install_set_request import InstallSetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InstallSetRequest from a JSON string
install_set_request_instance = InstallSetRequest.from_json(json)
# print the JSON string representation of the object
print(InstallSetRequest.to_json())

# convert the object into a dict
install_set_request_dict = install_set_request_instance.to_dict()
# create an instance of InstallSetRequest from a dict
install_set_request_from_dict = InstallSetRequest.from_dict(install_set_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


