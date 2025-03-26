# InstallationSslCertificate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**installed** | **bool** | SSL certificate installation status | 
**self_signed** | **bool** | SSL certificate self-signature status | 
**actual** | **bool** | SSL certificate actuality status | 
**suitable_for_domain** | **bool** | Status of SSL certificate suitability for domain | 
**issuer_name** | **str** | SSL certificate issuer name | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_ssl_certificate import InstallationSslCertificate

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationSslCertificate from a JSON string
installation_ssl_certificate_instance = InstallationSslCertificate.from_json(json)
# print the JSON string representation of the object
print(InstallationSslCertificate.to_json())

# convert the object into a dict
installation_ssl_certificate_dict = installation_ssl_certificate_instance.to_dict()
# create an instance of InstallationSslCertificate from a dict
installation_ssl_certificate_from_dict = InstallationSslCertificate.from_dict(installation_ssl_certificate_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


