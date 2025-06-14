# geocoding-nominatim-cache-client-python
An API for caching geocoding locations as fetched from Nominatim.

This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

- API version: 1.0
- Package version: 1.0.0
- Generator version: 7.13.0
- Build package: org.openapitools.codegen.languages.PythonClientCodegen

## Requirements.

Python 3.9+

## Installation & Usage
### pip install

If the python package is hosted on a repository, you can install directly using:

```sh
pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
```
(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)

Then import the package:
```python
import geocoding_nominatim_cache_client_python
```

### Setuptools

Install via [Setuptools](http://pypi.python.org/pypi/setuptools).

```sh
python setup.py install --user
```
(or `sudo python setup.py install` to install the package for all users)

Then import the package:
```python
import geocoding_nominatim_cache_client_python
```

### Tests

Execute `pytest` to run the tests.

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```python

import geocoding_nominatim_cache_client_python
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
    except ApiException as e:
        print("Exception when calling DefaultApi->locations_place_get: %s\n" % e)

```

## Documentation for API Endpoints

All URIs are relative to *http://localhost:8080*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*DefaultApi* | [**locations_place_get**](docs/DefaultApi.md#locations_place_get) | **GET** /locations/{place} | Get location coordinates for a placename


## Documentation For Models

 - [LocationLocation](docs/LocationLocation.md)
 - [MainErrorResponse](docs/MainErrorResponse.md)


<a id="documentation-for-authorization"></a>
## Documentation For Authorization

Endpoints do not require authorization.


## Author




