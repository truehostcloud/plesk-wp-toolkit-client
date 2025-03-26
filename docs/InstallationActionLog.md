# InstallationActionLog


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available** | **bool** | Availability of action log feature | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_action_log import InstallationActionLog

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationActionLog from a JSON string
installation_action_log_instance = InstallationActionLog.from_json(json)
# print the JSON string representation of the object
print(InstallationActionLog.to_json())

# convert the object into a dict
installation_action_log_dict = installation_action_log_instance.to_dict()
# create an instance of InstallationActionLog from a dict
installation_action_log_from_dict = InstallationActionLog.from_dict(installation_action_log_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


