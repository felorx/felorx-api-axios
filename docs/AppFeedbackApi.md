# AppFeedbackApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createAppFeedback**](#createappfeedback) | **POST** /api/app/app-feedback | 创建反馈（允许匿名用户提交）|
|[**deleteAppFeedbackById**](#deleteappfeedbackbyid) | **DELETE** /api/app/app-feedback/{id} | |
|[**getAppFeedbackById**](#getappfeedbackbyid) | **GET** /api/app/app-feedback/{id} | |
|[**getAppFeedbackList**](#getappfeedbacklist) | **GET** /api/app/app-feedback | |
|[**markAsProcessed**](#markasprocessed) | **POST** /api/app/app-feedback/{id}/mark-as-processed | |
|[**reply**](#reply) | **POST** /api/app/app-feedback/{id}/reply | |

# **createAppFeedback**
> AppFeedbackDto createAppFeedback()


### Example

```typescript
import {
    AppFeedbackApi,
    Configuration,
    CreateAppFeedbackDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppFeedbackApi(configuration);

let createAppFeedbackDto: CreateAppFeedbackDto; // (optional)

const { status, data } = await apiInstance.createAppFeedback(
    createAppFeedbackDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createAppFeedbackDto** | **CreateAppFeedbackDto**|  | |


### Return type

**AppFeedbackDto**

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

# **deleteAppFeedbackById**
> deleteAppFeedbackById()


### Example

```typescript
import {
    AppFeedbackApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppFeedbackApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteAppFeedbackById(
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

# **getAppFeedbackById**
> AppFeedbackDto getAppFeedbackById()


### Example

```typescript
import {
    AppFeedbackApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppFeedbackApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getAppFeedbackById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AppFeedbackDto**

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

# **getAppFeedbackList**
> AppFeedbackDtoPagedResultDto getAppFeedbackList()


### Example

```typescript
import {
    AppFeedbackApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppFeedbackApi(configuration);

let appId: string; //应用ID（必填，只有应用创建者可以查看） (optional) (default to undefined)
let type: AppFeedbackType; //反馈类型 (optional) (default to undefined)
let status: AppFeedbackStatus; //反馈状态 (optional) (default to undefined)
let sorting: string; // (optional) (default to undefined)
let skipCount: number; // (optional) (default to undefined)
let maxResultCount: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAppFeedbackList(
    appId,
    type,
    status,
    sorting,
    skipCount,
    maxResultCount
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appId** | [**string**] | 应用ID（必填，只有应用创建者可以查看） | (optional) defaults to undefined|
| **type** | **AppFeedbackType** | 反馈类型 | (optional) defaults to undefined|
| **status** | **AppFeedbackStatus** | 反馈状态 | (optional) defaults to undefined|
| **sorting** | [**string**] |  | (optional) defaults to undefined|
| **skipCount** | [**number**] |  | (optional) defaults to undefined|
| **maxResultCount** | [**number**] |  | (optional) defaults to undefined|


### Return type

**AppFeedbackDtoPagedResultDto**

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

# **markAsProcessed**
> AppFeedbackDto markAsProcessed()


### Example

```typescript
import {
    AppFeedbackApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppFeedbackApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.markAsProcessed(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AppFeedbackDto**

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

# **reply**
> AppFeedbackDto reply()


### Example

```typescript
import {
    AppFeedbackApi,
    Configuration,
    ReplyAppFeedbackDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppFeedbackApi(configuration);

let id: string; // (default to undefined)
let replyAppFeedbackDto: ReplyAppFeedbackDto; // (optional)

const { status, data } = await apiInstance.reply(
    id,
    replyAppFeedbackDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **replyAppFeedbackDto** | **ReplyAppFeedbackDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AppFeedbackDto**

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

