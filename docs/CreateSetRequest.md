# CreateSetRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **str** | Title | 
**plugins** | [**List[PluginAssetDetails]**](PluginAssetDetails.md) | Plugins | 
**themes** | [**List[ThemeAssetDetails]**](ThemeAssetDetails.md) | Themes | 

## Example

```python
from plesk_wp_toolkit_client.models.create_set_request import CreateSetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateSetRequest from a JSON string
create_set_request_instance = CreateSetRequest.from_json(json)
# print the JSON string representation of the object
print(CreateSetRequest.to_json())

# convert the object into a dict
create_set_request_dict = create_set_request_instance.to_dict()
# create an instance of CreateSetRequest from a dict
create_set_request_from_dict = CreateSetRequest.from_dict(create_set_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


