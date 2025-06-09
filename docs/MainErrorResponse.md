# MainErrorResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**error** | **str** |  | [optional] 

## Example

```python
from geocoding_nominatim_cache_client_python.models.main_error_response import MainErrorResponse

# TODO update the JSON string below
json = "{}"
# create an instance of MainErrorResponse from a JSON string
main_error_response_instance = MainErrorResponse.from_json(json)
# print the JSON string representation of the object
print(MainErrorResponse.to_json())

# convert the object into a dict
main_error_response_dict = main_error_response_instance.to_dict()
# create an instance of MainErrorResponse from a dict
main_error_response_from_dict = MainErrorResponse.from_dict(main_error_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


