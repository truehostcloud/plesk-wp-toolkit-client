# PluginAssetDetails


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**slug** | **str** | Slug | 
**status** | **bool** | Should be active after installation | 

## Example

```python
from plesk_wp_toolkit_client.models.plugin_asset_details import PluginAssetDetails

# TODO update the JSON string below
json = "{}"
# create an instance of PluginAssetDetails from a JSON string
plugin_asset_details_instance = PluginAssetDetails.from_json(json)
# print the JSON string representation of the object
print(PluginAssetDetails.to_json())

# convert the object into a dict
plugin_asset_details_dict = plugin_asset_details_instance.to_dict()
# create an instance of PluginAssetDetails from a dict
plugin_asset_details_from_dict = PluginAssetDetails.from_dict(plugin_asset_details_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


