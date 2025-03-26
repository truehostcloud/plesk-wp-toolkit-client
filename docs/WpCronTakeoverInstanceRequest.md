# WpCronTakeoverInstanceRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **bool** | Status | [optional] 
**task_replacement_status** | **bool** | Status | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.wp_cron_takeover_instance_request import WpCronTakeoverInstanceRequest

# TODO update the JSON string below
json = "{}"
# create an instance of WpCronTakeoverInstanceRequest from a JSON string
wp_cron_takeover_instance_request_instance = WpCronTakeoverInstanceRequest.from_json(json)
# print the JSON string representation of the object
print(WpCronTakeoverInstanceRequest.to_json())

# convert the object into a dict
wp_cron_takeover_instance_request_dict = wp_cron_takeover_instance_request_instance.to_dict()
# create an instance of WpCronTakeoverInstanceRequest from a dict
wp_cron_takeover_instance_request_from_dict = WpCronTakeoverInstanceRequest.from_dict(wp_cron_takeover_instance_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


