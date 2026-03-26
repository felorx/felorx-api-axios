# DeployRecordApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createDeployRecord**](#createdeployrecord) | **POST** /api/app/deploy-record | |
|[**deleteDeployRecordById**](#deletedeployrecordbyid) | **DELETE** /api/app/deploy-record/{id} | |
|[**getByCiDeployId**](#getbycideployid) | **GET** /api/app/deploy-record/by-ci-deploy-id/{ciDeployId} | |
|[**getDeployRecordById**](#getdeployrecordbyid) | **GET** /api/app/deploy-record/{id} | |
|[**getDeployRecordList**](#getdeployrecordlist) | **GET** /api/app/deploy-record | |
|[**getLatest**](#getlatest) | **GET** /api/app/deploy-record/latest/{appId} | |
|[**getListByBuildRecordId**](#getlistbybuildrecordid) | **GET** /api/app/deploy-record/by-build-record-id/{buildRecordId} | |
|[**markAsCanceled**](#markascanceled) | **POST** /api/app/deploy-record/{id}/mark-as-canceled | |
|[**markAsDeploying**](#markasdeploying) | **POST** /api/app/deploy-record/{id}/mark-as-deploying | |
|[**markAsFailed**](#markasfailed) | **POST** /api/app/deploy-record/{id}/mark-as-failed | |
|[**markAsSucceeded**](#markassucceeded) | **POST** /api/app/deploy-record/{id}/mark-as-succeeded | |
|[**updateDeployRecord**](#updatedeployrecord) | **PUT** /api/app/deploy-record/{id} | |

# **createDeployRecord**
> DeployRecordDto createDeployRecord()


### Example

```typescript
import {
    DeployRecordApi,
    Configuration,
    CreateDeployRecordDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new DeployRecordApi(configuration);

let createDeployRecordDto: CreateDeployRecordDto; // (optional)

const { status, data } = await apiInstance.createDeployRecord(
    createDeployRecordDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createDeployRecordDto** | **CreateDeployRecordDto**|  | |


### Return type

**DeployRecordDto**

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

# **deleteDeployRecordById**
> deleteDeployRecordById()


### Example

```typescript
import {
    DeployRecordApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new DeployRecordApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteDeployRecordById(
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

# **getByCiDeployId**
> DeployRecordDto getByCiDeployId()


### Example

```typescript
import {
    DeployRecordApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new DeployRecordApi(configuration);

let ciDeployId: string; // (default to undefined)

const { status, data } = await apiInstance.getByCiDeployId(
    ciDeployId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **ciDeployId** | [**string**] |  | defaults to undefined|


### Return type

**DeployRecordDto**

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

# **getDeployRecordById**
> DeployRecordDto getDeployRecordById()


### Example

```typescript
import {
    DeployRecordApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new DeployRecordApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getDeployRecordById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**DeployRecordDto**

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

# **getDeployRecordList**
> DeployRecordDtoPagedResultDto getDeployRecordList()


### Example

```typescript
import {
    DeployRecordApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new DeployRecordApi(configuration);

let appId: string; //应用ID (optional) (default to undefined)
let status: DeployStatus; //部署状态 (optional) (default to undefined)
let platform: AppPlatform; //目标平台 (optional) (default to undefined)
let environment: string; //部署环境 (optional) (default to undefined)
let version: string; //版本号 (optional) (default to undefined)
let buildRecordId: string; //构建记录ID (optional) (default to undefined)
let sorting: string; // (optional) (default to undefined)
let skipCount: number; // (optional) (default to undefined)
let maxResultCount: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.getDeployRecordList(
    appId,
    status,
    platform,
    environment,
    version,
    buildRecordId,
    sorting,
    skipCount,
    maxResultCount
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appId** | [**string**] | 应用ID | (optional) defaults to undefined|
| **status** | **DeployStatus** | 部署状态 | (optional) defaults to undefined|
| **platform** | **AppPlatform** | 目标平台 | (optional) defaults to undefined|
| **environment** | [**string**] | 部署环境 | (optional) defaults to undefined|
| **version** | [**string**] | 版本号 | (optional) defaults to undefined|
| **buildRecordId** | [**string**] | 构建记录ID | (optional) defaults to undefined|
| **sorting** | [**string**] |  | (optional) defaults to undefined|
| **skipCount** | [**number**] |  | (optional) defaults to undefined|
| **maxResultCount** | [**number**] |  | (optional) defaults to undefined|


### Return type

**DeployRecordDtoPagedResultDto**

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
> DeployRecordDto getLatest()


### Example

```typescript
import {
    DeployRecordApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new DeployRecordApi(configuration);

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

**DeployRecordDto**

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

# **getListByBuildRecordId**
> Array<DeployRecordDto> getListByBuildRecordId()


### Example

```typescript
import {
    DeployRecordApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new DeployRecordApi(configuration);

let buildRecordId: string; // (default to undefined)

const { status, data } = await apiInstance.getListByBuildRecordId(
    buildRecordId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **buildRecordId** | [**string**] |  | defaults to undefined|


### Return type

**Array<DeployRecordDto>**

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
> DeployRecordDto markAsCanceled()


### Example

```typescript
import {
    DeployRecordApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new DeployRecordApi(configuration);

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

**DeployRecordDto**

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

# **markAsDeploying**
> DeployRecordDto markAsDeploying()


### Example

```typescript
import {
    DeployRecordApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new DeployRecordApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.markAsDeploying(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**DeployRecordDto**

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
> DeployRecordDto markAsFailed()


### Example

```typescript
import {
    DeployRecordApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new DeployRecordApi(configuration);

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

**DeployRecordDto**

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
> DeployRecordDto markAsSucceeded()


### Example

```typescript
import {
    DeployRecordApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new DeployRecordApi(configuration);

let id: string; // (default to undefined)
let deployUrl: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.markAsSucceeded(
    id,
    deployUrl
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **deployUrl** | [**string**] |  | (optional) defaults to undefined|


### Return type

**DeployRecordDto**

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

# **updateDeployRecord**
> DeployRecordDto updateDeployRecord()


### Example

```typescript
import {
    DeployRecordApi,
    Configuration,
    UpdateDeployRecordDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new DeployRecordApi(configuration);

let id: string; // (default to undefined)
let updateDeployRecordDto: UpdateDeployRecordDto; // (optional)

const { status, data } = await apiInstance.updateDeployRecord(
    id,
    updateDeployRecordDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateDeployRecordDto** | **UpdateDeployRecordDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**DeployRecordDto**

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

