# AppPricingItemApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createAppPricingItem**](#createapppricingitem) | **POST** /api/app/app-pricing-item | |
|[**deleteAppPricingItemById**](#deleteapppricingitembyid) | **DELETE** /api/app/app-pricing-item/{id} | |
|[**getAppPricingItemById**](#getapppricingitembyid) | **GET** /api/app/app-pricing-item/{id} | |
|[**getAppPricingItemList**](#getapppricingitemlist) | **GET** /api/app/app-pricing-item | |
|[**updateAppPricingItem**](#updateapppricingitem) | **PUT** /api/app/app-pricing-item/{id} | |

# **createAppPricingItem**
> AppPricingItemDto createAppPricingItem()


### Example

```typescript
import {
    AppPricingItemApi,
    Configuration,
    CreateOrUpdateAppPricingItemDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppPricingItemApi(configuration);

let createOrUpdateAppPricingItemDto: CreateOrUpdateAppPricingItemDto; // (optional)

const { status, data } = await apiInstance.createAppPricingItem(
    createOrUpdateAppPricingItemDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateAppPricingItemDto** | **CreateOrUpdateAppPricingItemDto**|  | |


### Return type

**AppPricingItemDto**

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**403** | Forbidden |  -  |
|**401** | Unauthorized |  -  |
|**400** | Bad Request |  -  |
|**404** | Not Found |  -  |
|**501** | Server Error |  -  |
|**500** | Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteAppPricingItemById**
> deleteAppPricingItemById()


### Example

```typescript
import {
    AppPricingItemApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppPricingItemApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteAppPricingItemById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

void (empty response body)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**403** | Forbidden |  -  |
|**401** | Unauthorized |  -  |
|**400** | Bad Request |  -  |
|**404** | Not Found |  -  |
|**501** | Server Error |  -  |
|**500** | Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAppPricingItemById**
> AppPricingItemDto getAppPricingItemById()


### Example

```typescript
import {
    AppPricingItemApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppPricingItemApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getAppPricingItemById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AppPricingItemDto**

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**403** | Forbidden |  -  |
|**401** | Unauthorized |  -  |
|**400** | Bad Request |  -  |
|**404** | Not Found |  -  |
|**501** | Server Error |  -  |
|**500** | Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAppPricingItemList**
> Array<AppPricingItemDto> getAppPricingItemList()


### Example

```typescript
import {
    AppPricingItemApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppPricingItemApi(configuration);

const { status, data } = await apiInstance.getAppPricingItemList();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<AppPricingItemDto>**

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**403** | Forbidden |  -  |
|**401** | Unauthorized |  -  |
|**400** | Bad Request |  -  |
|**404** | Not Found |  -  |
|**501** | Server Error |  -  |
|**500** | Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateAppPricingItem**
> AppPricingItemDto updateAppPricingItem()


### Example

```typescript
import {
    AppPricingItemApi,
    Configuration,
    CreateOrUpdateAppPricingItemDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppPricingItemApi(configuration);

let id: string; // (default to undefined)
let createOrUpdateAppPricingItemDto: CreateOrUpdateAppPricingItemDto; // (optional)

const { status, data } = await apiInstance.updateAppPricingItem(
    id,
    createOrUpdateAppPricingItemDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateAppPricingItemDto** | **CreateOrUpdateAppPricingItemDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AppPricingItemDto**

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |
|**403** | Forbidden |  -  |
|**401** | Unauthorized |  -  |
|**400** | Bad Request |  -  |
|**404** | Not Found |  -  |
|**501** | Server Error |  -  |
|**500** | Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

