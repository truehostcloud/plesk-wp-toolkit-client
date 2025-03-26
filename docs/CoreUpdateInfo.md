# CoreUpdateInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**update** | **bool** | WordPress core update is required | 
**restore_point** | **bool** | Restore point creation required | 

## Example

```python
from plesk_wp_toolkit_client.models.core_update_info import CoreUpdateInfo

# TODO update the JSON string below
json = "{}"
# create an instance of CoreUpdateInfo from a JSON string
core_update_info_instance = CoreUpdateInfo.from_json(json)
# print the JSON string representation of the object
print(CoreUpdateInfo.to_json())

# convert the object into a dict
core_update_info_dict = core_update_info_instance.to_dict()
# create an instance of CoreUpdateInfo from a dict
core_update_info_from_dict = CoreUpdateInfo.from_dict(core_update_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


