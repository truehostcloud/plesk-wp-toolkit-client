# WordPressAsset


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**author** | [**WordPressAssetAuthor**](WordPressAssetAuthor.md) |  | 
**downloaded** | **int** | Number of downloads | 
**installed** | **bool** | Asset is installed or not | 
**logo_url** | **str** | URL to a WordPress logo | 
**preview_url** | **str** | URL to a preview page | 
**rating** | [**WordPressAssetRating**](WordPressAssetRating.md) |  | 
**requires** | **str** | Required WordPress version | 
**screenshot_url** | **str** | URL to an asset icon or screenshot | 
**screenshots** | [**List[WordPressAssetScreenshotsInner]**](WordPressAssetScreenshotsInner.md) |  | 
**short_description** | **str** | Asset description | 
**sections** | [**List[WordPressAssetSection]**](WordPressAssetSection.md) |  | 
**slug** | **str** | Asset slug | 
**tested** | **str** | Tested WordPress version | 
**title** | **str** | Asset name | 
**updated** | **str** | Last update date | 
**version** | **str** | Asset version | 

## Example

```python
from plesk_wp_toolkit_client.models.word_press_asset import WordPressAsset

# TODO update the JSON string below
json = "{}"
# create an instance of WordPressAsset from a JSON string
word_press_asset_instance = WordPressAsset.from_json(json)
# print the JSON string representation of the object
print(WordPressAsset.to_json())

# convert the object into a dict
word_press_asset_dict = word_press_asset_instance.to_dict()
# create an instance of WordPressAsset from a dict
word_press_asset_from_dict = WordPressAsset.from_dict(word_press_asset_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


