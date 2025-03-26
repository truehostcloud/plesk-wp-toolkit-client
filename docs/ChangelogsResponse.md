# ChangelogsResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**changelog** | **str** |  | 

## Example

```python
from plesk_wp_toolkit_client.models.changelogs_response import ChangelogsResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ChangelogsResponse from a JSON string
changelogs_response_instance = ChangelogsResponse.from_json(json)
# print the JSON string representation of the object
print(ChangelogsResponse.to_json())

# convert the object into a dict
changelogs_response_dict = changelogs_response_instance.to_dict()
# create an instance of ChangelogsResponse from a dict
changelogs_response_from_dict = ChangelogsResponse.from_dict(changelogs_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


