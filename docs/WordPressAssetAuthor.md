# WordPressAssetAuthor


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Author name | 
**profile** | **str** | URL to an author profile | 

## Example

```python
from plesk_wp_toolkit_client.models.word_press_asset_author import WordPressAssetAuthor

# TODO update the JSON string below
json = "{}"
# create an instance of WordPressAssetAuthor from a JSON string
word_press_asset_author_instance = WordPressAssetAuthor.from_json(json)
# print the JSON string representation of the object
print(WordPressAssetAuthor.to_json())

# convert the object into a dict
word_press_asset_author_dict = word_press_asset_author_instance.to_dict()
# create an instance of WordPressAssetAuthor from a dict
word_press_asset_author_from_dict = WordPressAssetAuthor.from_dict(word_press_asset_author_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


