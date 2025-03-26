# InstallationAssetInstallRequest

Install an asset from WordPress repository

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**slug** | **str** | Asset slug | 
**status** | **bool** | Activate or not the asset after upload | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_asset_install_request import InstallationAssetInstallRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationAssetInstallRequest from a JSON string
installation_asset_install_request_instance = InstallationAssetInstallRequest.from_json(json)
# print the JSON string representation of the object
print(InstallationAssetInstallRequest.to_json())

# convert the object into a dict
installation_asset_install_request_dict = installation_asset_install_request_instance.to_dict()
# create an instance of InstallationAssetInstallRequest from a dict
installation_asset_install_request_from_dict = InstallationAssetInstallRequest.from_dict(installation_asset_install_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


