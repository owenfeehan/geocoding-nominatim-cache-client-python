# geocoding_nominatim_cache_client_python.DefaultApi

All URIs are relative to *http://localhost:8080*

Method | HTTP request | Description
------------- | ------------- | -------------
[**locations_place_get**](DefaultApi.md#locations_place_get) | **GET** /locations/{place} | Get location coordinates for a placename


# **locations_place_get**
> LocationLocation locations_place_get(place)

Get location coordinates for a placename

get location coordinates and a canonical placename from a placename-query-string

### Example


```python
import geocoding_nominatim_cache_client_python
from geocoding_nominatim_cache_client_python.models.location_location import LocationLocation
from geocoding_nominatim_cache_client_python.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:8080
# See configuration.py for a list of all supported configuration parameters.
configuration = geocoding_nominatim_cache_client_python.Configuration(
    host = "http://localhost:8080"
)


# Enter a context with an instance of the API client
with geocoding_nominatim_cache_client_python.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = geocoding_nominatim_cache_client_python.DefaultApi(api_client)
    place = 'place_example' # str | query indicating a place or address

    try:
        # Get location coordinates for a placename
        api_response = api_instance.locations_place_get(place)
        print("The response of DefaultApi->locations_place_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->locations_place_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **place** | **str**| query indicating a place or address | 

### Return type

[**LocationLocation**](LocationLocation.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |
**400** | Bad Request |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

