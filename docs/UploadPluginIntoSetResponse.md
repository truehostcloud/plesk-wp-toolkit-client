# UploadPluginIntoSetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **bool** | Plugin active status | 
**id** | **int** | Asset id in set | 
**uploaded** | **object** | File uploaded status | 
**slug** | **str** | Plugin slug | 
**title** | **str** | Plugin title | 

## Example

```python
from plesk_wp_toolkit_client.models.upload_plugin_into_set_response import UploadPluginIntoSetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of UploadPluginIntoSetResponse from a JSON string
upload_plugin_into_set_response_instance = UploadPluginIntoSetResponse.from_json(json)
# print the JSON string representation of the object
print(UploadPluginIntoSetResponse.to_json())

# convert the object into a dict
upload_plugin_into_set_response_dict = upload_plugin_into_set_response_instance.to_dict()
# create an instance of UploadPluginIntoSetResponse from a dict
upload_plugin_into_set_response_from_dict = UploadPluginIntoSetResponse.from_dict(upload_plugin_into_set_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


