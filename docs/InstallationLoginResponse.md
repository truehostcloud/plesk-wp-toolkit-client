# InstallationLoginResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**link** | **str** | Login link to WordPress admin area | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_login_response import InstallationLoginResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationLoginResponse from a JSON string
installation_login_response_instance = InstallationLoginResponse.from_json(json)
# print the JSON string representation of the object
print(InstallationLoginResponse.to_json())

# convert the object into a dict
installation_login_response_dict = installation_login_response_instance.to_dict()
# create an instance of InstallationLoginResponse from a dict
installation_login_response_from_dict = InstallationLoginResponse.from_dict(installation_login_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


