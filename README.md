# byoa-sample-algorithm

This repository contains a scaffold for the respository structure required for Euro Data Cube - Insights On Demand (aka BYOA Bring Your Own Algorithm).

A (simplified) version to calculate a [Maximum Chlorophyll Index (MCI)](https://eurodatacube.com/marketplace/notebooks/getting-started/EDC_Sentinel_Hub-XCUBE_integration.ipynb) together with a (crude) pricing model based on the selected area is used as sample.

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
        "name": "Spatial Resolution",
        "id": "spatial_res",
        "type": "float",
        "description": "Spatial Resolution",
        "optional": true
    }
]
```
