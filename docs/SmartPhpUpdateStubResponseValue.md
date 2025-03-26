# SmartPhpUpdateStubResponseValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**new_subdomain** | [**SmartPhpUpdateStubResponseValueNewSubdomain**](SmartPhpUpdateStubResponseValueNewSubdomain.md) |  | 
**php** | [**SmartPhpUpdateStubPhpResponse**](SmartPhpUpdateStubPhpResponse.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.smart_php_update_stub_response_value import SmartPhpUpdateStubResponseValue

# TODO update the JSON string below
json = "{}"
# create an instance of SmartPhpUpdateStubResponseValue from a JSON string
smart_php_update_stub_response_value_instance = SmartPhpUpdateStubResponseValue.from_json(json)
# print the JSON string representation of the object
print(SmartPhpUpdateStubResponseValue.to_json())

# convert the object into a dict
smart_php_update_stub_response_value_dict = smart_php_update_stub_response_value_instance.to_dict()
# create an instance of SmartPhpUpdateStubResponseValue from a dict
smart_php_update_stub_response_value_from_dict = SmartPhpUpdateStubResponseValue.from_dict(smart_php_update_stub_response_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


