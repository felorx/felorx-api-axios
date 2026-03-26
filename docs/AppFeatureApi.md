# AppFeatureApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createAppFeature**](#createappfeature) | **POST** /api/app/app-feature | |
|[**deleteAppFeatureById**](#deleteappfeaturebyid) | **DELETE** /api/app/app-feature/{id} | |
|[**getAppFeatureList**](#getappfeaturelist) | **GET** /api/app/app-feature | |
|[**updateAppFeature**](#updateappfeature) | **PUT** /api/app/app-feature/{id} | |

# **createAppFeature**
> AppFeatureDto createAppFeature()


### Example

```typescript
import {
    AppFeatureApi,
    Configuration,
    CreateOrUpdateAppFeatureDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppFeatureApi(configuration);

let createOrUpdateAppFeatureDto: CreateOrUpdateAppFeatureDto; // (optional)

const { status, data } = await apiInstance.createAppFeature(
    createOrUpdateAppFeatureDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateAppFeatureDto** | **CreateOrUpdateAppFeatureDto**|  | |


### Return type

**AppFeatureDto**

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

# **deleteAppFeatureById**
> deleteAppFeatureById()


### Example

```typescript
import {
    AppFeatureApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppFeatureApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteAppFeatureById(
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

# **getAppFeatureList**
> AppFeatureDtoPagedResultDto getAppFeatureList()


### Example

```typescript
import {
    AppFeatureApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppFeatureApi(configuration);

let appId: string; // (optional) (default to undefined)
let sorting: string; // (optional) (default to undefined)
let skipCount: number; // (optional) (default to undefined)
let maxResultCount: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAppFeatureList(
    appId,
    sorting,
    skipCount,
    maxResultCount
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appId** | [**string**] |  | (optional) defaults to undefined|
| **sorting** | [**string**] |  | (optional) defaults to undefined|
| **skipCount** | [**number**] |  | (optional) defaults to undefined|
| **maxResultCount** | [**number**] |  | (optional) defaults to undefined|


### Return type

**AppFeatureDtoPagedResultDto**

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

# **updateAppFeature**
> AppFeatureDto updateAppFeature()


### Example

```typescript
import {
    AppFeatureApi,
    Configuration,
    CreateOrUpdateAppFeatureDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppFeatureApi(configuration);

let id: string; // (default to undefined)
let createOrUpdateAppFeatureDto: CreateOrUpdateAppFeatureDto; // (optional)

const { status, data } = await apiInstance.updateAppFeature(
    id,
    createOrUpdateAppFeatureDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateAppFeatureDto** | **CreateOrUpdateAppFeatureDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AppFeatureDto**

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

