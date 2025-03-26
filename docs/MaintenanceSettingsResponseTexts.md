# MaintenanceSettingsResponseTexts

Change the text displayed on the maintenance screen

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **str** | Browser page title | 
**header** | **str** | Text block 1 (bigger font) | 
**subheader** | **str** | Text block 2 (smaller font) | 

## Example

```python
from plesk_wp_toolkit_client.models.maintenance_settings_response_texts import MaintenanceSettingsResponseTexts

# TODO update the JSON string below
json = "{}"
# create an instance of MaintenanceSettingsResponseTexts from a JSON string
maintenance_settings_response_texts_instance = MaintenanceSettingsResponseTexts.from_json(json)
# print the JSON string representation of the object
print(MaintenanceSettingsResponseTexts.to_json())

# convert the object into a dict
maintenance_settings_response_texts_dict = maintenance_settings_response_texts_instance.to_dict()
# create an instance of MaintenanceSettingsResponseTexts from a dict
maintenance_settings_response_texts_from_dict = MaintenanceSettingsResponseTexts.from_dict(maintenance_settings_response_texts_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


