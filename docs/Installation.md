# Installation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Installation ID in WP Toolkit database | 
**title** | **str** | WordPress site title | 
**url** | **str** | WordPress site URL | 
**version** | **str** | WordPress version | 
**path** | **str** | Local path to the WordPress site | 
**labels** | [**List[InstallationLabel]**](InstallationLabel.md) |  | 
**display_title** | **str** | WP Toolkit installation display title | 
**server** | **str** | Server name for remote installations | 
**error_message** | **str** | Error message | 
**installation_type** | **str** | WordPress installation type | 
**domain** | [**InstallationDomain**](InstallationDomain.md) |  | 
**screenshot** | [**InstallationScreenshot**](InstallationScreenshot.md) |  | 
**owner** | [**InstallationOwner**](InstallationOwner.md) |  | 
**features** | [**InstallationFeatures**](InstallationFeatures.md) |  | 
**status** | [**InstallationStatus**](InstallationStatus.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.installation import Installation

# TODO update the JSON string below
json = "{}"
# create an instance of Installation from a JSON string
installation_instance = Installation.from_json(json)
# print the JSON string representation of the object
print(Installation.to_json())

# convert the object into a dict
installation_dict = installation_instance.to_dict()
# create an instance of Installation from a dict
installation_from_dict = Installation.from_dict(installation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


