# SecurityMeasuresInstallationStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Installation ID | 
**display_title** | **str** | WordPress site title | 
**security_status** | [**InstallationSecurityStatusEnum**](InstallationSecurityStatusEnum.md) |  | 
**resolve_applicable** | **bool** | Applying of security measures might be disabled by the server administrator | 
**check_applicable** | **bool** | Checking security measure status might be disabled by the server administrator | 
**revert_applicable** | **bool** | Reverting security measures might be disabled by the server administrator | 
**last_security_check_timestamp** | **int** | Timestamp | 
**tasks** | [**SecurityMeasuresInstallationStatusTasks**](SecurityMeasuresInstallationStatusTasks.md) |  | 
**security_measures** | [**List[InstallationSecurityMeasure]**](InstallationSecurityMeasure.md) |  | 
**vulnerable** | **bool** | Installation vulnerability status | 

## Example

```python
from plesk_wp_toolkit_client.models.security_measures_installation_status import SecurityMeasuresInstallationStatus

# TODO update the JSON string below
json = "{}"
# create an instance of SecurityMeasuresInstallationStatus from a JSON string
security_measures_installation_status_instance = SecurityMeasuresInstallationStatus.from_json(json)
# print the JSON string representation of the object
print(SecurityMeasuresInstallationStatus.to_json())

# convert the object into a dict
security_measures_installation_status_dict = security_measures_installation_status_instance.to_dict()
# create an instance of SecurityMeasuresInstallationStatus from a dict
security_measures_installation_status_from_dict = SecurityMeasuresInstallationStatus.from_dict(security_measures_installation_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


