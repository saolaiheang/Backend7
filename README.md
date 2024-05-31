# AgroMarked Stories API
This API allows you to manage and retrieve AgroMarket stories. Below are the available endpoints and their functionalities.
### Endpoints
```
https://jolly-angel-aabddcd512.strapiapp.com/
```
### Get All AgroMarket
```
GET /api/categories
```
Example:https://jolly-angel-aabddcd512.strapiapp.com/api/categories

Returns a list of all AgroMarket.

### Get a Single AgroMarket

```
GET /api/categories/{id}
```
Example:https://jolly-angel-aabddcd512.strapiapp.com/api/categories/1

Returns a single AgroMarket by ID.

### Sort AgroMarket by Price(order: 'asc' or 'desc')

```
GET /api/categories/sortByPrice/{order}
```

Example: https://categories-api.vercel.app/api/categories/sortByPrice/asc

Returns a sorted list of AgroMarket by Price (ascending or descending).

### Sort AgroMarkey by Created Date

```
GET /api/categories/sortByCreatedAt/{order}
```

Example:https://categories-api.vercel.app/api/categories/sortByCreatedAt/asc

Returns a sorted list of AgroMarket by created date (ascending or descending).

### Usage

Make requests to the respective endpoints using your preferred HTTP client.

### Response Format

The API responses will be in JSON format and follow this structure:

```
{
            "id": 1,
            "attributes": {
                "Name": "Mango",
                "Price": 2.5,
                "Organic": true,
                "OriginProvince": "Kampong Speu",
                "OwnerID": 1,
                "ProductID": 1,
                "Quantity": "100",
                "createdAt": "2024-05-21T06:04:14.380Z",
                "updatedAt": "2024-05-21T06:04:17.946Z",
                "publishedAt": "2024-05-21T06:04:17.917Z",
                "images": {
                    "data": [
                        {
                            "id": 1,
                            "attributes": {
                                "name": "Mango.jpg",
                                "alternativeText": null,
                                "caption": null,
                                "width": 680,
                                "height": 490,
                                "formats": {
                                    "small": {
                                        "ext": ".jpg",
                                        "url": "https://jolly-angel-aabddcd512.media.strapiapp.com/small_Mango_3091489cca.jpg",
                                        "hash": "small_Mango_3091489cca",
                                        "mime": "image/jpeg",
                                        "name": "small_Mango.jpg",
                                        "path": null,
                                        "size": 16.56,
                                        "width": 500,
                                        "height": 360,
                                        "sizeInBytes": 16563
                                    },
                                    "thumbnail": {
                                        "ext": ".jpg",
                                        "url": "https://jolly-angel-aabddcd512.media.strapiapp.com/thumbnail_Mango_3091489cca.jpg",
                                        "hash": "thumbnail_Mango_3091489cca",
                                        "mime": "image/jpeg",
                                        "name": "thumbnail_Mango.jpg",
                                        "path": null,
                                        "size": 4.74,
                                        "width": 216,
                                        "height": 156,
                                        "sizeInBytes": 4738
                                    }
                                },
                                "hash": "Mango_3091489cca",
                                "ext": ".jpg",
                                "mime": "image/jpeg",
                                "size": 26.63,
                                "url": "https://jolly-angel-aabddcd512.media.strapiapp.com/Mango_3091489cca.jpg",
                                "previewUrl": null,
                                "provider": "strapi-provider-upload-strapi-cloud",
                                "provider_metadata": null,
                                "createdAt": "2024-05-21T06:03:57.132Z",
                                "updatedAt": "2024-05-21T06:03:57.132Z"
                            }
                        }
                    ]
                },
                "CategoryID": {
                    "data": {
                        "id": 1,
                        "attributes": {
                            "Name": "Fruit",
                            "createdAt": "2024-05-21T04:17:41.945Z",
                            "updatedAt": "2024-05-21T04:17:45.637Z",
                            "publishedAt": "2024-05-21T04:17:45.631Z"
                        }
                    }
                },
                "strapi_stage": {
                    "data": null
                },
                "strapi_assignee": {
                    "data": null
                }
            }
        },
```
