# SmartUpdateResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Installation ID | 
**display_title** | **str** | WordPress site display title | 
**task_status** | **str** | Current status of Smart Update task | 
**clone** | [**SmartUpdateCloneInstallation**](SmartUpdateCloneInstallation.md) |  | 
**details** | [**List[SmartUpdatePageDetails]**](SmartUpdatePageDetails.md) |  | 
**created_at** | **datetime** | Date and time when Smart Update result was created | 

## Example

```python
from plesk_wp_toolkit_client.models.smart_update_result import SmartUpdateResult

# TODO update the JSON string below
json = "{}"
# create an instance of SmartUpdateResult from a JSON string
smart_update_result_instance = SmartUpdateResult.from_json(json)
# print the JSON string representation of the object
print(SmartUpdateResult.to_json())

# convert the object into a dict
smart_update_result_dict = smart_update_result_instance.to_dict()
# create an instance of SmartUpdateResult from a dict
smart_update_result_from_dict = SmartUpdateResult.from_dict(smart_update_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


