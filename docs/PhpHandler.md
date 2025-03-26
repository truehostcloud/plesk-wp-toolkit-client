# PhpHandler

WordPress site PHP handler

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**identifier** | **str** | WordPress site PHP handler identifier | 
**name** | **str** | WordPress site PHP handler name | 
**version** | **str** | WordPress site PHP handler version | 

## Example

```python
from plesk_wp_toolkit_client.models.php_handler import PhpHandler

# TODO update the JSON string below
json = "{}"
# create an instance of PhpHandler from a JSON string
php_handler_instance = PhpHandler.from_json(json)
# print the JSON string representation of the object
print(PhpHandler.to_json())

# convert the object into a dict
php_handler_dict = php_handler_instance.to_dict()
# create an instance of PhpHandler from a dict
php_handler_from_dict = PhpHandler.from_dict(php_handler_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


