# BuildRecordApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createBuildRecord**](#createbuildrecord) | **POST** /api/app/build-record | |
|[**deleteBuildRecordById**](#deletebuildrecordbyid) | **DELETE** /api/app/build-record/{id} | |
|[**getBuildRecordById**](#getbuildrecordbyid) | **GET** /api/app/build-record/{id} | |
|[**getBuildRecordList**](#getbuildrecordlist) | **GET** /api/app/build-record | |
|[**getByCiBuildId**](#getbycibuildid) | **GET** /api/app/build-record/by-ci-build-id/{ciBuildId} | |
|[**getLatest**](#getlatest) | **GET** /api/app/build-record/latest/{appId} | |
|[**markAsBuilding**](#markasbuilding) | **POST** /api/app/build-record/{id}/mark-as-building | |
|[**markAsCanceled**](#markascanceled) | **POST** /api/app/build-record/{id}/mark-as-canceled | |
|[**markAsFailed**](#markasfailed) | **POST** /api/app/build-record/{id}/mark-as-failed | |
|[**markAsSucceeded**](#markassucceeded) | **POST** /api/app/build-record/{id}/mark-as-succeeded | |
|[**updateBuildRecord**](#updatebuildrecord) | **PUT** /api/app/build-record/{id} | |

# **createBuildRecord**
> BuildRecordDto createBuildRecord()


### Example

```typescript
import {
    BuildRecordApi,
    Configuration,
    CreateBuildRecordDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new BuildRecordApi(configuration);

let createBuildRecordDto: CreateBuildRecordDto; // (optional)

const { status, data } = await apiInstance.createBuildRecord(
    createBuildRecordDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createBuildRecordDto** | **CreateBuildRecordDto**|  | |


### Return type

**BuildRecordDto**

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

# **deleteBuildRecordById**
> deleteBuildRecordById()


### Example

```typescript
import {
    BuildRecordApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new BuildRecordApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteBuildRecordById(
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

# **getBuildRecordById**
> BuildRecordDto getBuildRecordById()


### Example

```typescript
import {
    BuildRecordApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new BuildRecordApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getBuildRecordById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**BuildRecordDto**

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

# **getBuildRecordList**
> BuildRecordDtoPagedResultDto getBuildRecordList()


### Example

```typescript
import {
    BuildRecordApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new BuildRecordApi(configuration);

let appId: string; //应用ID (optional) (default to undefined)
let status: BuildStatus; //构建状态 (optional) (default to undefined)
let platform: AppPlatform; //目标平台 (optional) (default to undefined)
let environment: string; //环境 (optional) (default to undefined)
let version: string; //版本号 (optional) (default to undefined)
let branch: string; //分支名称 (optional) (default to undefined)
let sorting: string; // (optional) (default to undefined)
let skipCount: number; // (optional) (default to undefined)
let maxResultCount: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.getBuildRecordList(
    appId,
    status,
    platform,
    environment,
    version,
    branch,
    sorting,
    skipCount,
    maxResultCount
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appId** | [**string**] | 应用ID | (optional) defaults to undefined|
| **status** | **BuildStatus** | 构建状态 | (optional) defaults to undefined|
| **platform** | **AppPlatform** | 目标平台 | (optional) defaults to undefined|
| **environment** | [**string**] | 环境 | (optional) defaults to undefined|
| **version** | [**string**] | 版本号 | (optional) defaults to undefined|
| **branch** | [**string**] | 分支名称 | (optional) defaults to undefined|
| **sorting** | [**string**] |  | (optional) defaults to undefined|
| **skipCount** | [**number**] |  | (optional) defaults to undefined|
| **maxResultCount** | [**number**] |  | (optional) defaults to undefined|


### Return type

**BuildRecordDtoPagedResultDto**

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

# **getByCiBuildId**
> BuildRecordDto getByCiBuildId()


### Example

```typescript
import {
    BuildRecordApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new BuildRecordApi(configuration);

let ciBuildId: string; // (default to undefined)

const { status, data } = await apiInstance.getByCiBuildId(
    ciBuildId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **ciBuildId** | [**string**] |  | defaults to undefined|


### Return type

**BuildRecordDto**

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
> BuildRecordDto getLatest()


### Example

```typescript
import {
    BuildRecordApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new BuildRecordApi(configuration);

let appId: string; // (default to undefined)
let platform: AppPlatform; // (optional) (default to undefined)
let environment: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getLatest(
    appId,
    platform,
    environment
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appId** | [**string**] |  | defaults to undefined|
| **platform** | **AppPlatform** |  | (optional) defaults to undefined|
| **environment** | [**string**] |  | (optional) defaults to undefined|


### Return type

**BuildRecordDto**

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

# **markAsBuilding**
> BuildRecordDto markAsBuilding()


### Example

```typescript
import {
    BuildRecordApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new BuildRecordApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.markAsBuilding(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**BuildRecordDto**

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

# **markAsCanceled**
> BuildRecordDto markAsCanceled()


### Example

```typescript
import {
    BuildRecordApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new BuildRecordApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.markAsCanceled(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**BuildRecordDto**

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

# **markAsFailed**
> BuildRecordDto markAsFailed()


### Example

```typescript
import {
    BuildRecordApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new BuildRecordApi(configuration);

let id: string; // (default to undefined)
let errorMessage: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.markAsFailed(
    id,
    errorMessage
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **errorMessage** | [**string**] |  | (optional) defaults to undefined|


### Return type

**BuildRecordDto**

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

# **markAsSucceeded**
> BuildRecordDto markAsSucceeded()


### Example

```typescript
import {
    BuildRecordApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new BuildRecordApi(configuration);

let id: string; // (default to undefined)
let artifactUrl: string; // (optional) (default to undefined)
let artifactSize: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.markAsSucceeded(
    id,
    artifactUrl,
    artifactSize
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **artifactUrl** | [**string**] |  | (optional) defaults to undefined|
| **artifactSize** | [**number**] |  | (optional) defaults to undefined|


### Return type

**BuildRecordDto**

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

# **updateBuildRecord**
> BuildRecordDto updateBuildRecord()


### Example

```typescript
import {
    BuildRecordApi,
    Configuration,
    UpdateBuildRecordDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new BuildRecordApi(configuration);

let id: string; // (default to undefined)
let updateBuildRecordDto: UpdateBuildRecordDto; // (optional)

const { status, data } = await apiInstance.updateBuildRecord(
    id,
    updateBuildRecordDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateBuildRecordDto** | **UpdateBuildRecordDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**BuildRecordDto**

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

