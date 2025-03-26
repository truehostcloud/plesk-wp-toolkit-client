# InstallationOwner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Account ID | 
**login** | **str** | Username | 
**name** | **str** | Account name | 
**url** | **str** | URL to account management page in the panel | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_owner import InstallationOwner

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationOwner from a JSON string
installation_owner_instance = InstallationOwner.from_json(json)
# print the JSON string representation of the object
print(InstallationOwner.to_json())

# convert the object into a dict
installation_owner_dict = installation_owner_instance.to_dict()
# create an instance of InstallationOwner from a dict
installation_owner_from_dict = InstallationOwner.from_dict(installation_owner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


