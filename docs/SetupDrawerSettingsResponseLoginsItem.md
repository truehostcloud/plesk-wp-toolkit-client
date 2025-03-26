# SetupDrawerSettingsResponseLoginsItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**login** | **str** |  | 
**title** | **str** |  | 

## Example

```python
from plesk_wp_toolkit_client.models.setup_drawer_settings_response_logins_item import SetupDrawerSettingsResponseLoginsItem

# TODO update the JSON string below
json = "{}"
# create an instance of SetupDrawerSettingsResponseLoginsItem from a JSON string
setup_drawer_settings_response_logins_item_instance = SetupDrawerSettingsResponseLoginsItem.from_json(json)
# print the JSON string representation of the object
print(SetupDrawerSettingsResponseLoginsItem.to_json())

# convert the object into a dict
setup_drawer_settings_response_logins_item_dict = setup_drawer_settings_response_logins_item_instance.to_dict()
# create an instance of SetupDrawerSettingsResponseLoginsItem from a dict
setup_drawer_settings_response_logins_item_from_dict = SetupDrawerSettingsResponseLoginsItem.from_dict(setup_drawer_settings_response_logins_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


