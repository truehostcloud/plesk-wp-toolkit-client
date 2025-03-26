# WpCronTakeoverInstanceFeature


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available** | **bool** | Availability of wp-cron takeover feature | 
**status** | **bool** | Status | [optional] 
**task_replacement_status** | **bool** | Status | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.wp_cron_takeover_instance_feature import WpCronTakeoverInstanceFeature

# TODO update the JSON string below
json = "{}"
# create an instance of WpCronTakeoverInstanceFeature from a JSON string
wp_cron_takeover_instance_feature_instance = WpCronTakeoverInstanceFeature.from_json(json)
# print the JSON string representation of the object
print(WpCronTakeoverInstanceFeature.to_json())

# convert the object into a dict
wp_cron_takeover_instance_feature_dict = wp_cron_takeover_instance_feature_instance.to_dict()
# create an instance of WpCronTakeoverInstanceFeature from a dict
wp_cron_takeover_instance_feature_from_dict = WpCronTakeoverInstanceFeature.from_dict(wp_cron_takeover_instance_feature_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


