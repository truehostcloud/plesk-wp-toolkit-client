# SmartPhpUpdateResult


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Installation ID | 
**display_title** | **str** | WordPress site display title | 
**url** | **str** | WordPress site URL | 
**timestamp** | **int** | Time | 
**php_update_status** | [**InstallationSmartPhpUpdatesTaskStatusEnum**](InstallationSmartPhpUpdatesTaskStatusEnum.md) |  | 
**php_handler** | [**PhpHandler**](PhpHandler.md) |  | 
**target_php_handler** | [**PhpHandler**](PhpHandler.md) |  | 
**clone** | [**SmartPhpUpdateCloneInstallation**](SmartPhpUpdateCloneInstallation.md) |  | 
**details** | [**List[SmartUpdatePageDetails]**](SmartUpdatePageDetails.md) |  | 
**created_at** | **datetime** | Date and time when Smart PHP Update result was created | 

## Example

```python
from plesk_wp_toolkit_client.models.smart_php_update_result import SmartPhpUpdateResult

# TODO update the JSON string below
json = "{}"
# create an instance of SmartPhpUpdateResult from a JSON string
smart_php_update_result_instance = SmartPhpUpdateResult.from_json(json)
# print the JSON string representation of the object
print(SmartPhpUpdateResult.to_json())

# convert the object into a dict
smart_php_update_result_dict = smart_php_update_result_instance.to_dict()
# create an instance of SmartPhpUpdateResult from a dict
smart_php_update_result_from_dict = SmartPhpUpdateResult.from_dict(smart_php_update_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


