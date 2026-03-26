# AppAssetApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createAppAsset**](#createappasset) | **POST** /api/app/app-asset | |
|[**deleteAppAssetById**](#deleteappassetbyid) | **DELETE** /api/app/app-asset/{id} | |
|[**getListByAppLocaleId**](#getlistbyapplocaleid) | **GET** /api/app/app-asset/by-app-locale-id/{appLocaleId} | |
|[**updateAppAsset**](#updateappasset) | **PUT** /api/app/app-asset/{id} | |

# **createAppAsset**
> AppAssetDto createAppAsset()


### Example

```typescript
import {
    AppAssetApi,
    Configuration,
    CreateOrUpdateAppAssetDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppAssetApi(configuration);

let createOrUpdateAppAssetDto: CreateOrUpdateAppAssetDto; // (optional)

const { status, data } = await apiInstance.createAppAsset(
    createOrUpdateAppAssetDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateAppAssetDto** | **CreateOrUpdateAppAssetDto**|  | |


### Return type

**AppAssetDto**

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

# **deleteAppAssetById**
> deleteAppAssetById()


### Example

```typescript
import {
    AppAssetApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppAssetApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteAppAssetById(
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

# **getListByAppLocaleId**
> Array<AppAssetDto> getListByAppLocaleId()


### Example

```typescript
import {
    AppAssetApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppAssetApi(configuration);

let appLocaleId: string; // (default to undefined)

const { status, data } = await apiInstance.getListByAppLocaleId(
    appLocaleId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appLocaleId** | [**string**] |  | defaults to undefined|


### Return type

**Array<AppAssetDto>**

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

# **updateAppAsset**
> AppAssetDto updateAppAsset()


### Example

```typescript
import {
    AppAssetApi,
    Configuration,
    CreateOrUpdateAppAssetDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppAssetApi(configuration);

let id: string; // (default to undefined)
let createOrUpdateAppAssetDto: CreateOrUpdateAppAssetDto; // (optional)

const { status, data } = await apiInstance.updateAppAsset(
    id,
    createOrUpdateAppAssetDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateAppAssetDto** | **CreateOrUpdateAppAssetDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AppAssetDto**

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

