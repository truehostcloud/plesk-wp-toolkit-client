# RunSmartPhpUpdateRequestNewSubDomain

Create subdomain

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**parent_domain** | **str** | Under this domain will be created subdomain. ID on Plesk or domain name on cPanel. | 
**name** | **str** | Subdomain name. | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.run_smart_php_update_request_new_sub_domain import RunSmartPhpUpdateRequestNewSubDomain

# TODO update the JSON string below
json = "{}"
# create an instance of RunSmartPhpUpdateRequestNewSubDomain from a JSON string
run_smart_php_update_request_new_sub_domain_instance = RunSmartPhpUpdateRequestNewSubDomain.from_json(json)
# print the JSON string representation of the object
print(RunSmartPhpUpdateRequestNewSubDomain.to_json())

# convert the object into a dict
run_smart_php_update_request_new_sub_domain_dict = run_smart_php_update_request_new_sub_domain_instance.to_dict()
# create an instance of RunSmartPhpUpdateRequestNewSubDomain from a dict
run_smart_php_update_request_new_sub_domain_from_dict = RunSmartPhpUpdateRequestNewSubDomain.from_dict(run_smart_php_update_request_new_sub_domain_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


