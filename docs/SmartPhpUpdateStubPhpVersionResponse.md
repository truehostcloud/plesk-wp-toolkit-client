# SmartPhpUpdateStubPhpVersionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **str** |  | 
**title** | **str** |  | 
**eoled** | **bool** | EOL status of PHP version | 
**is_fpm_available** | **bool** | Available FPM handler | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.smart_php_update_stub_php_version_response import SmartPhpUpdateStubPhpVersionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SmartPhpUpdateStubPhpVersionResponse from a JSON string
smart_php_update_stub_php_version_response_instance = SmartPhpUpdateStubPhpVersionResponse.from_json(json)
# print the JSON string representation of the object
print(SmartPhpUpdateStubPhpVersionResponse.to_json())

# convert the object into a dict
smart_php_update_stub_php_version_response_dict = smart_php_update_stub_php_version_response_instance.to_dict()
# create an instance of SmartPhpUpdateStubPhpVersionResponse from a dict
smart_php_update_stub_php_version_response_from_dict = SmartPhpUpdateStubPhpVersionResponse.from_dict(smart_php_update_stub_php_version_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


