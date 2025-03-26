# InstallationWpCron


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available** | **bool** | Availability of wp-cron.php takeover feature | 
**status** | **bool** | Status of wp-cron.php takeover feature | 
**task_replacement_status** | **bool** | Status of replacement task creation | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_wp_cron import InstallationWpCron

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationWpCron from a JSON string
installation_wp_cron_instance = InstallationWpCron.from_json(json)
# print the JSON string representation of the object
print(InstallationWpCron.to_json())

# convert the object into a dict
installation_wp_cron_dict = installation_wp_cron_instance.to_dict()
# create an instance of InstallationWpCron from a dict
installation_wp_cron_from_dict = InstallationWpCron.from_dict(installation_wp_cron_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


