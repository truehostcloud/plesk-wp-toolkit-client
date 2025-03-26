# InstallationLabel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**color** | **str** |  | 
**name** | **str** |  | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_label import InstallationLabel

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationLabel from a JSON string
installation_label_instance = InstallationLabel.from_json(json)
# print the JSON string representation of the object
print(InstallationLabel.to_json())

# convert the object into a dict
installation_label_dict = installation_label_instance.to_dict()
# create an instance of InstallationLabel from a dict
installation_label_from_dict = InstallationLabel.from_dict(installation_label_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


