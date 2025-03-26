# RunSmartPhpUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**installation_id** | **int** | Installation ID | 
**new_sub_domain** | [**RunSmartPhpUpdateRequestNewSubDomain**](RunSmartPhpUpdateRequestNewSubDomain.md) |  | 
**php** | **str** | PHP handle identifier | 

## Example

```python
from plesk_wp_toolkit_client.models.run_smart_php_update_request import RunSmartPhpUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of RunSmartPhpUpdateRequest from a JSON string
run_smart_php_update_request_instance = RunSmartPhpUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(RunSmartPhpUpdateRequest.to_json())

# convert the object into a dict
run_smart_php_update_request_dict = run_smart_php_update_request_instance.to_dict()
# create an instance of RunSmartPhpUpdateRequest from a dict
run_smart_php_update_request_from_dict = RunSmartPhpUpdateRequest.from_dict(run_smart_php_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


