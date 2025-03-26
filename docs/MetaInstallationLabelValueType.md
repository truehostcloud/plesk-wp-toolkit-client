# MetaInstallationLabelValueType


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **str** |  | 
**meta** | [**MetaInstallationLabelValueTypeMeta**](MetaInstallationLabelValueTypeMeta.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.meta_installation_label_value_type import MetaInstallationLabelValueType

# TODO update the JSON string below
json = "{}"
# create an instance of MetaInstallationLabelValueType from a JSON string
meta_installation_label_value_type_instance = MetaInstallationLabelValueType.from_json(json)
# print the JSON string representation of the object
print(MetaInstallationLabelValueType.to_json())

# convert the object into a dict
meta_installation_label_value_type_dict = meta_installation_label_value_type_instance.to_dict()
# create an instance of MetaInstallationLabelValueType from a dict
meta_installation_label_value_type_from_dict = MetaInstallationLabelValueType.from_dict(meta_installation_label_value_type_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


