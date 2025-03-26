# FailedDependencyResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meta** | [**Meta**](Meta.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.failed_dependency_response import FailedDependencyResponse

# TODO update the JSON string below
json = "{}"
# create an instance of FailedDependencyResponse from a JSON string
failed_dependency_response_instance = FailedDependencyResponse.from_json(json)
# print the JSON string representation of the object
print(FailedDependencyResponse.to_json())

# convert the object into a dict
failed_dependency_response_dict = failed_dependency_response_instance.to_dict()
# create an instance of FailedDependencyResponse from a dict
failed_dependency_response_from_dict = FailedDependencyResponse.from_dict(failed_dependency_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


