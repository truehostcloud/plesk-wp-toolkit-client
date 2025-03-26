# InstallationCopyData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**applicable** | **bool** | Availability of data copy feature in the license | 
**available** | **bool** | Permission to use data copy feature by the server administrator | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_copy_data import InstallationCopyData

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationCopyData from a JSON string
installation_copy_data_instance = InstallationCopyData.from_json(json)
# print the JSON string representation of the object
print(InstallationCopyData.to_json())

# convert the object into a dict
installation_copy_data_dict = installation_copy_data_instance.to_dict()
# create an instance of InstallationCopyData from a dict
installation_copy_data_from_dict = InstallationCopyData.from_dict(installation_copy_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


