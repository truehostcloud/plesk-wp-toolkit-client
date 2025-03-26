# InstallationNginxCaching


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available** | **bool** | Availability of Nginx caching feature | 
**status** | **bool** | Nginx caching feature status | 
**web_server_settings_url** | **str** | URL to web server settings page | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_nginx_caching import InstallationNginxCaching

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationNginxCaching from a JSON string
installation_nginx_caching_instance = InstallationNginxCaching.from_json(json)
# print the JSON string representation of the object
print(InstallationNginxCaching.to_json())

# convert the object into a dict
installation_nginx_caching_dict = installation_nginx_caching_instance.to_dict()
# create an instance of InstallationNginxCaching from a dict
installation_nginx_caching_from_dict = InstallationNginxCaching.from_dict(installation_nginx_caching_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


