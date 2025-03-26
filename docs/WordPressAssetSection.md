# WordPressAssetSection


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content** | **str** | Section content in HTML format | 
**type** | **str** | Section type | 

## Example

```python
from plesk_wp_toolkit_client.models.word_press_asset_section import WordPressAssetSection

# TODO update the JSON string below
json = "{}"
# create an instance of WordPressAssetSection from a JSON string
word_press_asset_section_instance = WordPressAssetSection.from_json(json)
# print the JSON string representation of the object
print(WordPressAssetSection.to_json())

# convert the object into a dict
word_press_asset_section_dict = word_press_asset_section_instance.to_dict()
# create an instance of WordPressAssetSection from a dict
word_press_asset_section_from_dict = WordPressAssetSection.from_dict(word_press_asset_section_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


