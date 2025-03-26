# InstallationSynchronizeSiteUrl


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available** | **bool** | Availability of synchronize site URL feature | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_synchronize_site_url import InstallationSynchronizeSiteUrl

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationSynchronizeSiteUrl from a JSON string
installation_synchronize_site_url_instance = InstallationSynchronizeSiteUrl.from_json(json)
# print the JSON string representation of the object
print(InstallationSynchronizeSiteUrl.to_json())

# convert the object into a dict
installation_synchronize_site_url_dict = installation_synchronize_site_url_instance.to_dict()
# create an instance of InstallationSynchronizeSiteUrl from a dict
installation_synchronize_site_url_from_dict = InstallationSynchronizeSiteUrl.from_dict(installation_synchronize_site_url_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


