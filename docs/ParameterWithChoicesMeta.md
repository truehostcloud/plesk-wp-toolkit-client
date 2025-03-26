# ParameterWithChoicesMeta


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**choices** | [**List[ParameterWithChoicesMetaChoicesInner]**](ParameterWithChoicesMetaChoicesInner.md) | List of available choices | 

## Example

```python
from plesk_wp_toolkit_client.models.parameter_with_choices_meta import ParameterWithChoicesMeta

# TODO update the JSON string below
json = "{}"
# create an instance of ParameterWithChoicesMeta from a JSON string
parameter_with_choices_meta_instance = ParameterWithChoicesMeta.from_json(json)
# print the JSON string representation of the object
print(ParameterWithChoicesMeta.to_json())

# convert the object into a dict
parameter_with_choices_meta_dict = parameter_with_choices_meta_instance.to_dict()
# create an instance of ParameterWithChoicesMeta from a dict
parameter_with_choices_meta_from_dict = ParameterWithChoicesMeta.from_dict(parameter_with_choices_meta_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


