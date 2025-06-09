# LocationLocation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**display_name** | **str** |  | [optional] 
**lat** | **str** |  | [optional] 
**lon** | **str** |  | [optional] 

## Example

```python
from geocoding_nominatim_cache_client_python.models.location_location import LocationLocation

# TODO update the JSON string below
json = "{}"
# create an instance of LocationLocation from a JSON string
location_location_instance = LocationLocation.from_json(json)
# print the JSON string representation of the object
print(LocationLocation.to_json())

# convert the object into a dict
location_location_dict = location_location_instance.to_dict()
# create an instance of LocationLocation from a dict
location_location_from_dict = LocationLocation.from_dict(location_location_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


