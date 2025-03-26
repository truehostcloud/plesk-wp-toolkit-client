# CacheCleanerRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**installations_ids** | **List[int]** |  | 
**tags** | **List[str]** |  | [optional] 

## Example

```python
from plesk_wp_toolkit_client.models.cache_cleaner_request import CacheCleanerRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CacheCleanerRequest from a JSON string
cache_cleaner_request_instance = CacheCleanerRequest.from_json(json)
# print the JSON string representation of the object
print(CacheCleanerRequest.to_json())

# convert the object into a dict
cache_cleaner_request_dict = cache_cleaner_request_instance.to_dict()
# create an instance of CacheCleanerRequest from a dict
cache_cleaner_request_from_dict = CacheCleanerRequest.from_dict(cache_cleaner_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


