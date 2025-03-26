# SetupDrawerSettingsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**login** | **str** | Site administrator username to WordPress admin dashboard | [optional] 
**password** | **str** | Site administrator password to WordPress admin dashboard | [optional] 
**email** | **str** | Site admininistrator email | [optional] 
**language** | **str** | Installation language | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.setup_drawer_settings_request import SetupDrawerSettingsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SetupDrawerSettingsRequest from a JSON string
setup_drawer_settings_request_instance = SetupDrawerSettingsRequest.from_json(json)
# print the JSON string representation of the object
print(SetupDrawerSettingsRequest.to_json())

# convert the object into a dict
setup_drawer_settings_request_dict = setup_drawer_settings_request_instance.to_dict()
# create an instance of SetupDrawerSettingsRequest from a dict
setup_drawer_settings_request_from_dict = SetupDrawerSettingsRequest.from_dict(setup_drawer_settings_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


