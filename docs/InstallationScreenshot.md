# InstallationScreenshot


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **str** | Date and time the screenshot was taken | 
**url** | **str** | Screenshot URL | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_screenshot import InstallationScreenshot

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationScreenshot from a JSON string
installation_screenshot_instance = InstallationScreenshot.from_json(json)
# print the JSON string representation of the object
print(InstallationScreenshot.to_json())

# convert the object into a dict
installation_screenshot_dict = installation_screenshot_instance.to_dict()
# create an instance of InstallationScreenshot from a dict
installation_screenshot_from_dict = InstallationScreenshot.from_dict(installation_screenshot_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


