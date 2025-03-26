# MetaInstallationLabel


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | [**MetaInstallationLabelValue**](MetaInstallationLabelValue.md) |  | 
**meta** | **object** |  | 

## Example

```python
from plesk_wp_toolkit_client.models.meta_installation_label import MetaInstallationLabel

# TODO update the JSON string below
json = "{}"
# create an instance of MetaInstallationLabel from a JSON string
meta_installation_label_instance = MetaInstallationLabel.from_json(json)
# print the JSON string representation of the object
print(MetaInstallationLabel.to_json())

# convert the object into a dict
meta_installation_label_dict = meta_installation_label_instance.to_dict()
# create an instance of MetaInstallationLabel from a dict
meta_installation_label_from_dict = MetaInstallationLabel.from_dict(meta_installation_label_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


