# SetDetailsAssetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **str** | Title | 
**slug** | **str** | Slug | 
**status** | **bool** | Status | 
**uploaded** | **bool** | Is uploaded | 
**id** | **int** | ID | 

## Example

```python
from plesk_wp_toolkit_client.models.set_details_asset_response import SetDetailsAssetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SetDetailsAssetResponse from a JSON string
set_details_asset_response_instance = SetDetailsAssetResponse.from_json(json)
# print the JSON string representation of the object
print(SetDetailsAssetResponse.to_json())

# convert the object into a dict
set_details_asset_response_dict = set_details_asset_response_instance.to_dict()
# create an instance of SetDetailsAssetResponse from a dict
set_details_asset_response_from_dict = SetDetailsAssetResponse.from_dict(set_details_asset_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


