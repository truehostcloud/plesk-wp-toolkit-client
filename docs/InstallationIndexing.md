# InstallationIndexing


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **bool** | Status of search engine indexing feature | 

## Example

```python
from plesk_wp_toolkit_client.models.installation_indexing import InstallationIndexing

# TODO update the JSON string below
json = "{}"
# create an instance of InstallationIndexing from a JSON string
installation_indexing_instance = InstallationIndexing.from_json(json)
# print the JSON string representation of the object
print(InstallationIndexing.to_json())

# convert the object into a dict
installation_indexing_dict = installation_indexing_instance.to_dict()
# create an instance of InstallationIndexing from a dict
installation_indexing_from_dict = InstallationIndexing.from_dict(installation_indexing_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


