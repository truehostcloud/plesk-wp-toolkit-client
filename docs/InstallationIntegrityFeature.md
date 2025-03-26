# InstallationIntegrityFeature


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available** | **bool** | Availability of WordPress integrity check feature | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_integrity_feature import InstallationIntegrityFeature

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationIntegrityFeature from a JSON string
installation_integrity_feature_instance = InstallationIntegrityFeature.from_json(json)
# print the JSON string representation of the object
print(InstallationIntegrityFeature.to_json())

# convert the object into a dict
installation_integrity_feature_dict = installation_integrity_feature_instance.to_dict()
# create an instance of InstallationIntegrityFeature from a dict
installation_integrity_feature_from_dict = InstallationIntegrityFeature.from_dict(installation_integrity_feature_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


