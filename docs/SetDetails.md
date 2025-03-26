# SetDetails


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | ID | 
**title** | **str** | Set name | 
**plugins** | [**List[SetDetailsAssetResponse]**](SetDetailsAssetResponse.md) | Plugins | 
**themes** | [**List[SetDetailsAssetResponse]**](SetDetailsAssetResponse.md) | Themes | 

## Example

```python
from plesk_wp_toolkit_client.models.set_details import SetDetails

# TODO update the JSON string below
json = "{}"
# create an instance of SetDetails from a JSON string
set_details_instance = SetDetails.from_json(json)
# print the JSON string representation of the object
print(SetDetails.to_json())

# convert the object into a dict
set_details_dict = set_details_instance.to_dict()
# create an instance of SetDetails from a dict
set_details_from_dict = SetDetails.from_dict(set_details_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


