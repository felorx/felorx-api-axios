# AppReleaseApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createAppRelease**](#createapprelease) | **POST** /api/app/app-release | 创建新版本|
|[**deleteAppReleaseById**](#deleteappreleasebyid) | **DELETE** /api/app/app-release/{id} | 删除版本|
|[**getAppReleaseById**](#getappreleasebyid) | **GET** /api/app/app-release/{id} | 获取版本|
|[**getAppReleaseList**](#getappreleaselist) | **GET** /api/app/app-release | 获取版本列表|
|[**getLatest**](#getlatest) | **GET** /api/app/app-release/latest | 获取最新版本|
|[**getListByDeveloper**](#getlistbydeveloper) | **GET** /api/app/app-release/by-developer | 开发者获取版本列表（版本的创建者为当前用户）|
|[**updateAppRelease**](#updateapprelease) | **PUT** /api/app/app-release/{id} | 更新版本|

# **createAppRelease**
> AppReleaseDto createAppRelease()


### Example

```typescript
import {
    AppReleaseApi,
    Configuration,
    CreateOrUpdateAppReleaseDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppReleaseApi(configuration);

let createOrUpdateAppReleaseDto: CreateOrUpdateAppReleaseDto; // (optional)

const { status, data } = await apiInstance.createAppRelease(
    createOrUpdateAppReleaseDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateAppReleaseDto** | **CreateOrUpdateAppReleaseDto**|  | |


### Return type

**AppReleaseDto**

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

# **deleteAppReleaseById**
> deleteAppReleaseById()


### Example

```typescript
import {
    AppReleaseApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppReleaseApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteAppReleaseById(
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

# **getAppReleaseById**
> AppReleaseDto getAppReleaseById()


### Example

```typescript
import {
    AppReleaseApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppReleaseApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getAppReleaseById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AppReleaseDto**

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

# **getAppReleaseList**
> AppReleaseDtoPagedResultDto getAppReleaseList()


### Example

```typescript
import {
    AppReleaseApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppReleaseApi(configuration);

let appId: string; // (optional) (default to undefined)
let channel: ReleaseChannel; // (optional) (default to undefined)
let platform: string; // (optional) (default to undefined)
let publisher: string; // (optional) (default to undefined)
let sorting: string; // (optional) (default to undefined)
let skipCount: number; // (optional) (default to undefined)
let maxResultCount: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAppReleaseList(
    appId,
    channel,
    platform,
    publisher,
    sorting,
    skipCount,
    maxResultCount
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appId** | [**string**] |  | (optional) defaults to undefined|
| **channel** | **ReleaseChannel** |  | (optional) defaults to undefined|
| **platform** | [**string**] |  | (optional) defaults to undefined|
| **publisher** | [**string**] |  | (optional) defaults to undefined|
| **sorting** | [**string**] |  | (optional) defaults to undefined|
| **skipCount** | [**number**] |  | (optional) defaults to undefined|
| **maxResultCount** | [**number**] |  | (optional) defaults to undefined|


### Return type

**AppReleaseDtoPagedResultDto**

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

# **getLatest**
> AppReleaseDto getLatest()


### Example

```typescript
import {
    AppReleaseApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppReleaseApi(configuration);

let appName: string; // (optional) (default to undefined)
let platform: string; // (optional) (default to undefined)
let artifactType: string; // (optional) (default to undefined)
let publisher: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getLatest(
    appName,
    platform,
    artifactType,
    publisher
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appName** | [**string**] |  | (optional) defaults to undefined|
| **platform** | [**string**] |  | (optional) defaults to undefined|
| **artifactType** | [**string**] |  | (optional) defaults to undefined|
| **publisher** | [**string**] |  | (optional) defaults to undefined|


### Return type

**AppReleaseDto**

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

# **getListByDeveloper**
> AppReleaseDtoPagedResultDto getListByDeveloper()


### Example

```typescript
import {
    AppReleaseApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppReleaseApi(configuration);

let appId: string; // (optional) (default to undefined)
let channel: ReleaseChannel; // (optional) (default to undefined)
let platform: string; // (optional) (default to undefined)
let publisher: string; // (optional) (default to undefined)
let sorting: string; // (optional) (default to undefined)
let skipCount: number; // (optional) (default to undefined)
let maxResultCount: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.getListByDeveloper(
    appId,
    channel,
    platform,
    publisher,
    sorting,
    skipCount,
    maxResultCount
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appId** | [**string**] |  | (optional) defaults to undefined|
| **channel** | **ReleaseChannel** |  | (optional) defaults to undefined|
| **platform** | [**string**] |  | (optional) defaults to undefined|
| **publisher** | [**string**] |  | (optional) defaults to undefined|
| **sorting** | [**string**] |  | (optional) defaults to undefined|
| **skipCount** | [**number**] |  | (optional) defaults to undefined|
| **maxResultCount** | [**number**] |  | (optional) defaults to undefined|


### Return type

**AppReleaseDtoPagedResultDto**

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

# **updateAppRelease**
> AppReleaseDto updateAppRelease()


### Example

```typescript
import {
    AppReleaseApi,
    Configuration,
    CreateOrUpdateAppReleaseDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppReleaseApi(configuration);

let id: string; // (default to undefined)
let createOrUpdateAppReleaseDto: CreateOrUpdateAppReleaseDto; // (optional)

const { status, data } = await apiInstance.updateAppRelease(
    id,
    createOrUpdateAppReleaseDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateAppReleaseDto** | **CreateOrUpdateAppReleaseDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AppReleaseDto**

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

