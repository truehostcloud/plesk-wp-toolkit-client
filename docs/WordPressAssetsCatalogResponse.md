# WordPressAssetsCatalogResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total** | **int** | Total number of available assets | 
**items** | [**List[WordPressAsset]**](WordPressAsset.md) | List of available assets | 

## Example

```python
from plesk_wp_toolkit_client.models.word_press_assets_catalog_response import WordPressAssetsCatalogResponse

# TODO update the JSON string below
json = "{}"
# create an instance of WordPressAssetsCatalogResponse from a JSON string
word_press_assets_catalog_response_instance = WordPressAssetsCatalogResponse.from_json(json)
# print the JSON string representation of the object
print(WordPressAssetsCatalogResponse.to_json())

# convert the object into a dict
word_press_assets_catalog_response_dict = word_press_assets_catalog_response_instance.to_dict()
# create an instance of WordPressAssetsCatalogResponse from a dict
word_press_assets_catalog_response_from_dict = WordPressAssetsCatalogResponse.from_dict(word_press_assets_catalog_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


