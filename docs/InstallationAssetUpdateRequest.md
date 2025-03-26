# InstallationAssetUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**slug** | **str** | Asset slug | 
**auto_updates** | **bool** | New autoUpdate value | [optional] 
**status** | **bool** | New status value | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.installation_asset_update_request import InstallationAssetUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationAssetUpdateRequest from a JSON string
installation_asset_update_request_instance = InstallationAssetUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(InstallationAssetUpdateRequest.to_json())

# convert the object into a dict
installation_asset_update_request_dict = installation_asset_update_request_instance.to_dict()
# create an instance of InstallationAssetUpdateRequest from a dict
installation_asset_update_request_from_dict = InstallationAssetUpdateRequest.from_dict(installation_asset_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


