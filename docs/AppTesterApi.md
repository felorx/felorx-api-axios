# AppTesterApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**checkIsAppTester**](#checkisapptester) | **POST** /api/app/app-tester/check-is-app-tester | 检查用户是否是内测用户|
|[**createAppTester**](#createapptester) | **POST** /api/app/app-tester | 创建内测用户|
|[**deleteAppTesterById**](#deleteapptesterbyid) | **DELETE** /api/app/app-tester/{id} | 删除内测用户|
|[**getAppTesterById**](#getapptesterbyid) | **GET** /api/app/app-tester/{id} | 获取内测用户|
|[**getAppTesterList**](#getapptesterlist) | **GET** /api/app/app-tester | 获取内测用户列表|
|[**updateAppTester**](#updateapptester) | **PUT** /api/app/app-tester/{id} | 更新内测用户|

# **checkIsAppTester**
> boolean checkIsAppTester()


### Example

```typescript
import {
    AppTesterApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppTesterApi(configuration);

let appId: string; // (optional) (default to undefined)
let userId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.checkIsAppTester(
    appId,
    userId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appId** | [**string**] |  | (optional) defaults to undefined|
| **userId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**boolean**

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

# **createAppTester**
> AppTesterDto createAppTester()


### Example

```typescript
import {
    AppTesterApi,
    Configuration,
    CreateUpdateAppTesterDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppTesterApi(configuration);

let createUpdateAppTesterDto: CreateUpdateAppTesterDto; // (optional)

const { status, data } = await apiInstance.createAppTester(
    createUpdateAppTesterDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createUpdateAppTesterDto** | **CreateUpdateAppTesterDto**|  | |


### Return type

**AppTesterDto**

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

# **deleteAppTesterById**
> deleteAppTesterById()


### Example

```typescript
import {
    AppTesterApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppTesterApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteAppTesterById(
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

# **getAppTesterById**
> AppTesterDto getAppTesterById()


### Example

```typescript
import {
    AppTesterApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppTesterApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getAppTesterById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AppTesterDto**

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

# **getAppTesterList**
> AppTesterDtoPagedResultDto getAppTesterList()


### Example

```typescript
import {
    AppTesterApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppTesterApi(configuration);

let sorting: string; // (optional) (default to undefined)
let skipCount: number; // (optional) (default to undefined)
let maxResultCount: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAppTesterList(
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

**AppTesterDtoPagedResultDto**

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

# **updateAppTester**
> AppTesterDto updateAppTester()


### Example

```typescript
import {
    AppTesterApi,
    Configuration,
    CreateUpdateAppTesterDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppTesterApi(configuration);

let id: string; // (default to undefined)
let createUpdateAppTesterDto: CreateUpdateAppTesterDto; // (optional)

const { status, data } = await apiInstance.updateAppTester(
    id,
    createUpdateAppTesterDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createUpdateAppTesterDto** | **CreateUpdateAppTesterDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AppTesterDto**

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

