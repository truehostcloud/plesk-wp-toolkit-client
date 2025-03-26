# InstallationPathValidatorRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**domain** | **str** | Domain name | 
**installation_path** | **str** | Installation path relative to the root directory of the domain | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.installation_path_validator_request import InstallationPathValidatorRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationPathValidatorRequest from a JSON string
installation_path_validator_request_instance = InstallationPathValidatorRequest.from_json(json)
# print the JSON string representation of the object
print(InstallationPathValidatorRequest.to_json())

# convert the object into a dict
installation_path_validator_request_dict = installation_path_validator_request_instance.to_dict()
# create an instance of InstallationPathValidatorRequest from a dict
installation_path_validator_request_from_dict = InstallationPathValidatorRequest.from_dict(installation_path_validator_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


