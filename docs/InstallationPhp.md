# InstallationPhp


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**handler** | [**PhpHandler**](PhpHandler.md) |  | 
**unsupported** | **bool** | PHP version support status | 
**eoled** | **bool** | PHP version EOL status | 
**settings_url** | **str** | URL to PHP management page in the panel | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_php import InstallationPhp

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationPhp from a JSON string
installation_php_instance = InstallationPhp.from_json(json)
# print the JSON string representation of the object
print(InstallationPhp.to_json())

# convert the object into a dict
installation_php_dict = installation_php_instance.to_dict()
# create an instance of InstallationPhp from a dict
installation_php_from_dict = InstallationPhp.from_dict(installation_php_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


