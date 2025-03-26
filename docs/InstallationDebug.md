# InstallationDebug


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **bool** | WordPress debug feature status | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_debug import InstallationDebug

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationDebug from a JSON string
installation_debug_instance = InstallationDebug.from_json(json)
# print the JSON string representation of the object
print(InstallationDebug.to_json())

# convert the object into a dict
installation_debug_dict = installation_debug_instance.to_dict()
# create an instance of InstallationDebug from a dict
installation_debug_from_dict = InstallationDebug.from_dict(installation_debug_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


