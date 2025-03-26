# SmartPhpUpdateStubResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | [**SmartPhpUpdateStubResponseValue**](SmartPhpUpdateStubResponseValue.md) |  | 
**meta** | [**SmartPhpUpdateStubResponseMeta**](SmartPhpUpdateStubResponseMeta.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.smart_php_update_stub_response import SmartPhpUpdateStubResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SmartPhpUpdateStubResponse from a JSON string
smart_php_update_stub_response_instance = SmartPhpUpdateStubResponse.from_json(json)
# print the JSON string representation of the object
print(SmartPhpUpdateStubResponse.to_json())

# convert the object into a dict
smart_php_update_stub_response_dict = smart_php_update_stub_response_instance.to_dict()
# create an instance of SmartPhpUpdateStubResponse from a dict
smart_php_update_stub_response_from_dict = SmartPhpUpdateStubResponse.from_dict(smart_php_update_stub_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


