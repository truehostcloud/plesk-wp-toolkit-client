# WordPressAssetScreenshotsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**caption** | **str** | Screenshot caption | 
**src** | **str** | Screenshot URL | 

## Example

```python
from plesk_wp_toolkit_client.models.word_press_asset_screenshots_inner import WordPressAssetScreenshotsInner

# TODO update the JSON string below
json = "{}"
# create an instance of WordPressAssetScreenshotsInner from a JSON string
word_press_asset_screenshots_inner_instance = WordPressAssetScreenshotsInner.from_json(json)
# print the JSON string representation of the object
print(WordPressAssetScreenshotsInner.to_json())

# convert the object into a dict
word_press_asset_screenshots_inner_dict = word_press_asset_screenshots_inner_instance.to_dict()
# create an instance of WordPressAssetScreenshotsInner from a dict
word_press_asset_screenshots_inner_from_dict = WordPressAssetScreenshotsInner.from_dict(word_press_asset_screenshots_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


