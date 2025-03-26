# SmartPhpUpdateStubPhpResponseMeta


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**versions** | [**List[SmartPhpUpdateStubPhpVersionResponse]**](SmartPhpUpdateStubPhpVersionResponse.md) | Available versions of PHP handlers | 

## Example

```python
from plesk_wp_toolkit_client.models.smart_php_update_stub_php_response_meta import SmartPhpUpdateStubPhpResponseMeta

# TODO update the JSON string below
json = "{}"
# create an instance of SmartPhpUpdateStubPhpResponseMeta from a JSON string
smart_php_update_stub_php_response_meta_instance = SmartPhpUpdateStubPhpResponseMeta.from_json(json)
# print the JSON string representation of the object
print(SmartPhpUpdateStubPhpResponseMeta.to_json())

# convert the object into a dict
smart_php_update_stub_php_response_meta_dict = smart_php_update_stub_php_response_meta_instance.to_dict()
# create an instance of SmartPhpUpdateStubPhpResponseMeta from a dict
smart_php_update_stub_php_response_meta_from_dict = SmartPhpUpdateStubPhpResponseMeta.from_dict(smart_php_update_stub_php_response_meta_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


