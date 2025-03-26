# ThemeAssetDetails


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**slug** | **str** | Slug | 
**status** | **bool** | Should be active after installation | 

## Example

```python
from plesk_wp_toolkit_client.models.theme_asset_details import ThemeAssetDetails

# TODO update the JSON string below
json = "{}"
# create an instance of ThemeAssetDetails from a JSON string
theme_asset_details_instance = ThemeAssetDetails.from_json(json)
# print the JSON string representation of the object
print(ThemeAssetDetails.to_json())

# convert the object into a dict
theme_asset_details_dict = theme_asset_details_instance.to_dict()
# create an instance of ThemeAssetDetails from a dict
theme_asset_details_from_dict = ThemeAssetDetails.from_dict(theme_asset_details_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


