# InstallationSsl


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** | SSL status | 
**redirect_to_https_enabled** | **bool** | Redirect to HTTPS status | 
**url_protocol_https** | **bool** | Status of HTTPS in URL protocol | 
**certificate** | [**InstallationSslCertificate**](InstallationSslCertificate.md) |  | 
**enable_ssl_action_url** | **str** | URL for enabling SSL | 
**buy_or_install_ssl_action_url** | **str** | URL for installing SSL certificate | 
**enable_redirect_to_https_action_url** | **str** | URL for enabling redirect to HTTPS | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_ssl import InstallationSsl

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationSsl from a JSON string
installation_ssl_instance = InstallationSsl.from_json(json)
# print the JSON string representation of the object
print(InstallationSsl.to_json())

# convert the object into a dict
installation_ssl_dict = installation_ssl_instance.to_dict()
# create an instance of InstallationSsl from a dict
installation_ssl_from_dict = InstallationSsl.from_dict(installation_ssl_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


