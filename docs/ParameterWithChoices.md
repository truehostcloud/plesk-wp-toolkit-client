# ParameterWithChoices

Default value of installation parameter with the list of available choices

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **str** |  | 
**meta** | [**ParameterWithChoicesMeta**](ParameterWithChoicesMeta.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.parameter_with_choices import ParameterWithChoices

# TODO update the JSON string below
json = "{}"
# create an instance of ParameterWithChoices from a JSON string
parameter_with_choices_instance = ParameterWithChoices.from_json(json)
# print the JSON string representation of the object
print(ParameterWithChoices.to_json())

# convert the object into a dict
parameter_with_choices_dict = parameter_with_choices_instance.to_dict()
# create an instance of ParameterWithChoices from a dict
parameter_with_choices_from_dict = ParameterWithChoices.from_dict(parameter_with_choices_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


