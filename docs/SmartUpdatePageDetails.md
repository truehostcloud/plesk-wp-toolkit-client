# SmartUpdatePageDetails


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_url** | **str** | Page URL | 
**before** | [**SmartUpdatePageStatus**](SmartUpdatePageStatus.md) |  | 
**after** | [**SmartUpdatePageStatus**](SmartUpdatePageStatus.md) |  | 

## Example

```python
from plesk_wp_toolkit_client.models.smart_update_page_details import SmartUpdatePageDetails

# TODO update the JSON string below
json = "{}"
# create an instance of SmartUpdatePageDetails from a JSON string
smart_update_page_details_instance = SmartUpdatePageDetails.from_json(json)
# print the JSON string representation of the object
print(SmartUpdatePageDetails.to_json())

# convert the object into a dict
smart_update_page_details_dict = smart_update_page_details_instance.to_dict()
# create an instance of SmartUpdatePageDetails from a dict
smart_update_page_details_from_dict = SmartUpdatePageDetails.from_dict(smart_update_page_details_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


