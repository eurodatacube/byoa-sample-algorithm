# byoa-sample-algorithm

This repository contains a scaffold for the respository structure required for Bring Your Own Algorithm.

Please consult the [EDC documentation](https://eurodatacube.com/documentation/offer_algorithms_for_on_demand_data_generation) for more information.


### Parameters

This algorithm can be onboarded to the EDC platform using the following parameter specification:

```javascript
[
    {
        "name": "Area of interest",
        "id": "aoi",
        "type": "bbox",
        "description": "Area of interest",
        "optional": false
    },
    {
        "name": "Band name",
        "id": "band_name",
        "type": "string",
        "description": "Band name to use as data source",
        "optional": false,
        "restriction": {
             "type": "choice",
             "value": [
                 "B04",
                 "B05",
                 "B06"
             ]
        }
    },
    {
        "name": "Spatial Resolution",
        "id": "spatial_res",
        "type": "float",
        "description": "Spatial Resolution",
        "optional": false
    },
    {
        "name": "Max. cloud coverage",
        "id": "maxCC",
        "type": "float",
        "description": "Maximal cloud coverage in percentage",
        "optional": true,
        "restriction": {
          "type": "range",
          "value": [0, 100]
        }
    }
]
```
