# InstallationDomain


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Domain name | 
**url** | **str** | URL to domain management page in panel | 
**ssl_redirect_enabled** | **bool** | SSL redirect status on domain | 
**installations_limit** | **int** | Active limit of WordPress sites for a domain | 
**installations_count** | **int** | Count of installed WordPress sites on a domain | 
**ssl** | [**InstallationSsl**](InstallationSsl.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_domain import InstallationDomain

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationDomain from a JSON string
installation_domain_instance = InstallationDomain.from_json(json)
# print the JSON string representation of the object
print(InstallationDomain.to_json())

# convert the object into a dict
installation_domain_dict = installation_domain_instance.to_dict()
# create an instance of InstallationDomain from a dict
installation_domain_from_dict = InstallationDomain.from_dict(installation_domain_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


