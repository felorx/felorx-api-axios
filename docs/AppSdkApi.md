# AppSdkApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createAppSdk**](#createappsdk) | **POST** /api/app/app-sdk | |
|[**deleteAppSdkById**](#deleteappsdkbyid) | **DELETE** /api/app/app-sdk/{id} | |
|[**getAppSdkList**](#getappsdklist) | **GET** /api/app/app-sdk | |
|[**updateAppSdk**](#updateappsdk) | **PUT** /api/app/app-sdk/{id} | |

# **createAppSdk**
> AppSdkDto createAppSdk()


### Example

```typescript
import {
    AppSdkApi,
    Configuration,
    CreateOrUpdateAppSdkDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppSdkApi(configuration);

let createOrUpdateAppSdkDto: CreateOrUpdateAppSdkDto; // (optional)

const { status, data } = await apiInstance.createAppSdk(
    createOrUpdateAppSdkDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateAppSdkDto** | **CreateOrUpdateAppSdkDto**|  | |


### Return type

**AppSdkDto**

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

# **deleteAppSdkById**
> deleteAppSdkById()


### Example

```typescript
import {
    AppSdkApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppSdkApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteAppSdkById(
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

# **getAppSdkList**
> AppSdkDtoPagedResultDto getAppSdkList()


### Example

```typescript
import {
    AppSdkApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppSdkApi(configuration);

let sorting: string; // (optional) (default to undefined)
let skipCount: number; // (optional) (default to undefined)
let maxResultCount: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAppSdkList(
    sorting,
    skipCount,
    maxResultCount
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sorting** | [**string**] |  | (optional) defaults to undefined|
| **skipCount** | [**number**] |  | (optional) defaults to undefined|
| **maxResultCount** | [**number**] |  | (optional) defaults to undefined|


### Return type

**AppSdkDtoPagedResultDto**

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

# **updateAppSdk**
> AppSdkDto updateAppSdk()


### Example

```typescript
import {
    AppSdkApi,
    Configuration,
    CreateOrUpdateAppSdkDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppSdkApi(configuration);

let id: string; // (default to undefined)
let createOrUpdateAppSdkDto: CreateOrUpdateAppSdkDto; // (optional)

const { status, data } = await apiInstance.updateAppSdk(
    id,
    createOrUpdateAppSdkDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateAppSdkDto** | **CreateOrUpdateAppSdkDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AppSdkDto**

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

