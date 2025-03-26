# MetaInstallationLabels


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | [**List[MetaInstallationLabel]**](MetaInstallationLabel.md) |  | 
**meta** | [**MetaInstallationLabelsMeta**](MetaInstallationLabelsMeta.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.meta_installation_labels import MetaInstallationLabels

# TODO update the JSON string below
json = "{}"
# create an instance of MetaInstallationLabels from a JSON string
meta_installation_labels_instance = MetaInstallationLabels.from_json(json)
# print the JSON string representation of the object
print(MetaInstallationLabels.to_json())

# convert the object into a dict
meta_installation_labels_dict = meta_installation_labels_instance.to_dict()
# create an instance of MetaInstallationLabels from a dict
meta_installation_labels_from_dict = MetaInstallationLabels.from_dict(meta_installation_labels_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


