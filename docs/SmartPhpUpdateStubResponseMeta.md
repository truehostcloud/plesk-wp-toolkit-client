# SmartPhpUpdateStubResponseMeta


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tasks** | [**SmartPhpUpdateStubResponseMetaTasks**](SmartPhpUpdateStubResponseMetaTasks.md) |  | 
**task_status** | [**InstallationSmartPhpUpdatesTaskStatusEnum**](InstallationSmartPhpUpdatesTaskStatusEnum.md) |  | 
**limited** | **bool** | Smart PHP Update available for specific account configurations | 
**messages** | [**List[MessageResponse]**](MessageResponse.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.smart_php_update_stub_response_meta import SmartPhpUpdateStubResponseMeta

# TODO update the JSON string below
json = "{}"
# create an instance of SmartPhpUpdateStubResponseMeta from a JSON string
smart_php_update_stub_response_meta_instance = SmartPhpUpdateStubResponseMeta.from_json(json)
# print the JSON string representation of the object
print(SmartPhpUpdateStubResponseMeta.to_json())

# convert the object into a dict
smart_php_update_stub_response_meta_dict = smart_php_update_stub_response_meta_instance.to_dict()
# create an instance of SmartPhpUpdateStubResponseMeta from a dict
smart_php_update_stub_response_meta_from_dict = SmartPhpUpdateStubResponseMeta.from_dict(smart_php_update_stub_response_meta_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


