# MetaInstallationLabelValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | [**MetaInstallationLabelValueType**](MetaInstallationLabelValueType.md) |  | 
**color** | [**MetaInstallationLabelValueType**](MetaInstallationLabelValueType.md) |  | 
**name** | [**MetaInstallationLabelValueName**](MetaInstallationLabelValueName.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.meta_installation_label_value import MetaInstallationLabelValue

# TODO update the JSON string below
json = "{}"
# create an instance of MetaInstallationLabelValue from a JSON string
meta_installation_label_value_instance = MetaInstallationLabelValue.from_json(json)
# print the JSON string representation of the object
print(MetaInstallationLabelValue.to_json())

# convert the object into a dict
meta_installation_label_value_dict = meta_installation_label_value_instance.to_dict()
# create an instance of MetaInstallationLabelValue from a dict
meta_installation_label_value_from_dict = MetaInstallationLabelValue.from_dict(meta_installation_label_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


