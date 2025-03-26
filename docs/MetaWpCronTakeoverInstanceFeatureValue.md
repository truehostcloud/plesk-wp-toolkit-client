# MetaWpCronTakeoverInstanceFeatureValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**available** | [**MetaWpCronTakeoverInstanceFeatureValueAvailable**](MetaWpCronTakeoverInstanceFeatureValueAvailable.md) |  | 
**status** | [**MetaWpCronTakeoverInstanceFeatureValueAvailable**](MetaWpCronTakeoverInstanceFeatureValueAvailable.md) |  | [optional] 
**task_replacement_status** | [**MetaWpCronTakeoverInstanceFeatureValueTaskReplacementStatus**](MetaWpCronTakeoverInstanceFeatureValueTaskReplacementStatus.md) |  | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.meta_wp_cron_takeover_instance_feature_value import MetaWpCronTakeoverInstanceFeatureValue

# TODO update the JSON string below
json = "{}"
# create an instance of MetaWpCronTakeoverInstanceFeatureValue from a JSON string
meta_wp_cron_takeover_instance_feature_value_instance = MetaWpCronTakeoverInstanceFeatureValue.from_json(json)
# print the JSON string representation of the object
print(MetaWpCronTakeoverInstanceFeatureValue.to_json())

# convert the object into a dict
meta_wp_cron_takeover_instance_feature_value_dict = meta_wp_cron_takeover_instance_feature_value_instance.to_dict()
# create an instance of MetaWpCronTakeoverInstanceFeatureValue from a dict
meta_wp_cron_takeover_instance_feature_value_from_dict = MetaWpCronTakeoverInstanceFeatureValue.from_dict(meta_wp_cron_takeover_instance_feature_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


