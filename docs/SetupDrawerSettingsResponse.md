# SetupDrawerSettingsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**login_url** | **str** | Login URL to WordPress admin dashboard | 
**current_login** | **str** | Site administrator username for WordPress admin dashboard | 
**current_password** | **str** | Site administrator password for WordPress admin dashboard | 
**current_email** | **str** | Site administrator email | 
**current_language** | **str** | Installation language | 
**available_logins** | [**List[SetupDrawerSettingsResponseLoginsItem]**](SetupDrawerSettingsResponseLoginsItem.md) | List of available administrator accounts | 
**available_languages** | [**List[SetupDrawerSettingsResponseLanguagesItem]**](SetupDrawerSettingsResponseLanguagesItem.md) | List of available languages | 

## Example

```python
from plesk_wp_toolkit_client.models.setup_drawer_settings_response import SetupDrawerSettingsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SetupDrawerSettingsResponse from a JSON string
setup_drawer_settings_response_instance = SetupDrawerSettingsResponse.from_json(json)
# print the JSON string representation of the object
print(SetupDrawerSettingsResponse.to_json())

# convert the object into a dict
setup_drawer_settings_response_dict = setup_drawer_settings_response_instance.to_dict()
# create an instance of SetupDrawerSettingsResponse from a dict
setup_drawer_settings_response_from_dict = SetupDrawerSettingsResponse.from_dict(setup_drawer_settings_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


