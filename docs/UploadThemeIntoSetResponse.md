# UploadThemeIntoSetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **bool** | Theme active status | 
**id** | **int** | Asset id in set | 
**uploaded** | **object** | File uploaded status | 
**slug** | **str** | Theme slug | 
**title** | **str** | Theme title | 

## Example

```python
from plesk_wp_toolkit_client.models.upload_theme_into_set_response import UploadThemeIntoSetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of UploadThemeIntoSetResponse from a JSON string
upload_theme_into_set_response_instance = UploadThemeIntoSetResponse.from_json(json)
# print the JSON string representation of the object
print(UploadThemeIntoSetResponse.to_json())

# convert the object into a dict
upload_theme_into_set_response_dict = upload_theme_into_set_response_instance.to_dict()
# create an instance of UploadThemeIntoSetResponse from a dict
upload_theme_into_set_response_from_dict = UploadThemeIntoSetResponse.from_dict(upload_theme_into_set_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


