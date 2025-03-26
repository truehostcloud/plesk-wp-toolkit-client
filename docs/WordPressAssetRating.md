# WordPressAssetRating


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | **int** | Number of ratings | 
**score** | **float** | Rating score | 

## Example

```python
from plesk_wp_toolkit_client.models.word_press_asset_rating import WordPressAssetRating

# TODO update the JSON string below
json = "{}"
# create an instance of WordPressAssetRating from a JSON string
word_press_asset_rating_instance = WordPressAssetRating.from_json(json)
# print the JSON string representation of the object
print(WordPressAssetRating.to_json())

# convert the object into a dict
word_press_asset_rating_dict = word_press_asset_rating_instance.to_dict()
# create an instance of WordPressAssetRating from a dict
word_press_asset_rating_from_dict = WordPressAssetRating.from_dict(word_press_asset_rating_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


