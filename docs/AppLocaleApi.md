# AppLocaleApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createAppLocale**](#createapplocale) | **POST** /api/app/app-locale | |
|[**deleteAppLocaleById**](#deleteapplocalebyid) | **DELETE** /api/app/app-locale/{id} | |
|[**getListByAppIdGetApiAppAppLocaleByAppIdAppId**](#getlistbyappidgetapiappapplocalebyappidappid) | **GET** /api/app/app-locale/by-app-id/{appId} | |
|[**updateAppLocale**](#updateapplocale) | **PUT** /api/app/app-locale/{id} | |

# **createAppLocale**
> AppLocaleDto createAppLocale()


### Example

```typescript
import {
    AppLocaleApi,
    Configuration,
    CreateOrUpdateAppLocaleDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AppLocaleApi(configuration);

let createOrUpdateAppLocaleDto: CreateOrUpdateAppLocaleDto; // (optional)

const { status, data } = await apiInstance.createAppLocale(
    createOrUpdateAppLocaleDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateAppLocaleDto** | **CreateOrUpdateAppLocaleDto**|  | |


### Return type

**AppLocaleDto**

### Authorization

No authorization required

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

# **deleteAppLocaleById**
> deleteAppLocaleById()


### Example

```typescript
import {
    AppLocaleApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AppLocaleApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteAppLocaleById(
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

No authorization required

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

# **getListByAppIdGetApiAppAppLocaleByAppIdAppId**
> Array<AppLocaleDto> getListByAppIdGetApiAppAppLocaleByAppIdAppId()


### Example

```typescript
import {
    AppLocaleApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AppLocaleApi(configuration);

let appId: string; // (default to undefined)

const { status, data } = await apiInstance.getListByAppIdGetApiAppAppLocaleByAppIdAppId(
    appId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appId** | [**string**] |  | defaults to undefined|


### Return type

**Array<AppLocaleDto>**

### Authorization

No authorization required

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

# **updateAppLocale**
> AppLocaleDto updateAppLocale()


### Example

```typescript
import {
    AppLocaleApi,
    Configuration,
    CreateOrUpdateAppLocaleDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AppLocaleApi(configuration);

let id: string; // (default to undefined)
let createOrUpdateAppLocaleDto: CreateOrUpdateAppLocaleDto; // (optional)

const { status, data } = await apiInstance.updateAppLocale(
    id,
    createOrUpdateAppLocaleDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateAppLocaleDto** | **CreateOrUpdateAppLocaleDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AppLocaleDto**

### Authorization

No authorization required

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

