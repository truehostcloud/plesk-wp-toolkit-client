# ClonePathValidatorRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**domain** | **str** | Domain name | 
**installation_path** | **str** | Installation path of cloned WordPress site (relative to the root directory of the domain) | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.clone_path_validator_request import ClonePathValidatorRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ClonePathValidatorRequest from a JSON string
clone_path_validator_request_instance = ClonePathValidatorRequest.from_json(json)
# print the JSON string representation of the object
print(ClonePathValidatorRequest.to_json())

# convert the object into a dict
clone_path_validator_request_dict = clone_path_validator_request_instance.to_dict()
# create an instance of ClonePathValidatorRequest from a dict
clone_path_validator_request_from_dict = ClonePathValidatorRequest.from_dict(clone_path_validator_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


