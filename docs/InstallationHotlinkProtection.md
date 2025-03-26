# InstallationHotlinkProtection


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available** | **bool** | Availability of hotlink protection feature | 
**status** | **bool** | Hotlink protection feature status | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_hotlink_protection import InstallationHotlinkProtection

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationHotlinkProtection from a JSON string
installation_hotlink_protection_instance = InstallationHotlinkProtection.from_json(json)
# print the JSON string representation of the object
print(InstallationHotlinkProtection.to_json())

# convert the object into a dict
installation_hotlink_protection_dict = installation_hotlink_protection_instance.to_dict()
# create an instance of InstallationHotlinkProtection from a dict
installation_hotlink_protection_from_dict = InstallationHotlinkProtection.from_dict(installation_hotlink_protection_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


