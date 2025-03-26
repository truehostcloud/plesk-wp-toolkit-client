# InstallationClone


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**applicable** | **bool** | Availability of cloning feature in the license | 
**available** | **bool** | Permission to use cloning feature by the server administrator | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_clone import InstallationClone

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationClone from a JSON string
installation_clone_instance = InstallationClone.from_json(json)
# print the JSON string representation of the object
print(InstallationClone.to_json())

# convert the object into a dict
installation_clone_dict = installation_clone_instance.to_dict()
# create an instance of InstallationClone from a dict
installation_clone_from_dict = InstallationClone.from_dict(installation_clone_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


