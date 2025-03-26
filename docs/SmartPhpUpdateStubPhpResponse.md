# SmartPhpUpdateStubPhpResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **str** | PHP version value | 
**meta** | [**SmartPhpUpdateStubPhpResponseMeta**](SmartPhpUpdateStubPhpResponseMeta.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.smart_php_update_stub_php_response import SmartPhpUpdateStubPhpResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SmartPhpUpdateStubPhpResponse from a JSON string
smart_php_update_stub_php_response_instance = SmartPhpUpdateStubPhpResponse.from_json(json)
# print the JSON string representation of the object
print(SmartPhpUpdateStubPhpResponse.to_json())

# convert the object into a dict
smart_php_update_stub_php_response_dict = smart_php_update_stub_php_response_instance.to_dict()
# create an instance of SmartPhpUpdateStubPhpResponse from a dict
smart_php_update_stub_php_response_from_dict = SmartPhpUpdateStubPhpResponse.from_dict(smart_php_update_stub_php_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


