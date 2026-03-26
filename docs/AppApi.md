# AppApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createApp**](#createapp) | **POST** /api/app/app | |
|[**deleteAppById**](#deleteappbyid) | **DELETE** /api/app/app/{id} | |
|[**getAppById**](#getappbyid) | **GET** /api/app/app/{id} | |
|[**getAppList**](#getapplist) | **GET** /api/app/app | |
|[**getByName**](#getbyname) | **GET** /api/app/app/by-name | |
|[**getFeatureList**](#getfeaturelist) | **GET** /api/app/app/feature-list/{appId} | |
|[**getListByDeveloperAll**](#getlistbydeveloperall) | **GET** /api/app/app/by-developer-all | |
|[**getListPublic**](#getlistpublic) | **GET** /api/app/app/public | |
|[**getListWithUser**](#getlistwithuser) | **GET** /api/app/app/with-user | |
|[**getSdksById**](#getsdksbyid) | **GET** /api/app/app/sdks-by-id/{appId} | |
|[**getUploadCredentials**](#getuploadcredentials) | **GET** /api/app/app/upload-credentials | |
|[**getWithUser**](#getwithuser) | **GET** /api/app/app/{id}/with-user | |
|[**run**](#run) | **POST** /api/app/app/run | |
|[**updateApp**](#updateapp) | **PUT** /api/app/app/{id} | |
|[**updateRunState**](#updaterunstate) | **PUT** /api/app/app/{id}/run-state | |

# **createApp**
> AppDto createApp()


### Example

```typescript
import {
    AppApi,
    Configuration,
    CreateOrUpdateAppDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppApi(configuration);

let createOrUpdateAppDto: CreateOrUpdateAppDto; // (optional)

const { status, data } = await apiInstance.createApp(
    createOrUpdateAppDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateAppDto** | **CreateOrUpdateAppDto**|  | |


### Return type

**AppDto**

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

# **deleteAppById**
> deleteAppById()


### Example

```typescript
import {
    AppApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteAppById(
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

# **getAppById**
> AppDto getAppById()


### Example

```typescript
import {
    AppApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getAppById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AppDto**

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

# **getAppList**
> AppDtoPagedResultDto getAppList()


### Example

```typescript
import {
    AppApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppApi(configuration);

let creatorId: string; // (optional) (default to undefined)
let sorting: string; // (optional) (default to undefined)
let skipCount: number; // (optional) (default to undefined)
let maxResultCount: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAppList(
    creatorId,
    sorting,
    skipCount,
    maxResultCount
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **creatorId** | [**string**] |  | (optional) defaults to undefined|
| **sorting** | [**string**] |  | (optional) defaults to undefined|
| **skipCount** | [**number**] |  | (optional) defaults to undefined|
| **maxResultCount** | [**number**] |  | (optional) defaults to undefined|


### Return type

**AppDtoPagedResultDto**

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

# **getByName**
> AppDto getByName()


### Example

```typescript
import {
    AppApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppApi(configuration);

let name: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getByName(
    name
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **name** | [**string**] |  | (optional) defaults to undefined|


### Return type

**AppDto**

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

# **getFeatureList**
> Array<AppFeatureDto> getFeatureList()


### Example

```typescript
import {
    AppApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppApi(configuration);

let appId: string; // (default to undefined)
let env: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getFeatureList(
    appId,
    env
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appId** | [**string**] |  | defaults to undefined|
| **env** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Array<AppFeatureDto>**

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

# **getListByDeveloperAll**
> AppDtoPagedResultDto getListByDeveloperAll()


### Example

```typescript
import {
    AppApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppApi(configuration);

let developerAccount: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getListByDeveloperAll(
    developerAccount
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **developerAccount** | [**string**] |  | (optional) defaults to undefined|


### Return type

**AppDtoPagedResultDto**

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

# **getListPublic**
> AppDtoPagedResultDto getListPublic()


### Example

```typescript
import {
    AppApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppApi(configuration);

let type: string; // (optional) (default to undefined)
let developerAccount: string; // (optional) (default to undefined)
let currentAppName: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getListPublic(
    type,
    developerAccount,
    currentAppName
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **type** | [**string**] |  | (optional) defaults to undefined|
| **developerAccount** | [**string**] |  | (optional) defaults to undefined|
| **currentAppName** | [**string**] |  | (optional) defaults to undefined|


### Return type

**AppDtoPagedResultDto**

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

# **getListWithUser**
> AppWithUserDtoPagedResultDto getListWithUser()


### Example

```typescript
import {
    AppApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppApi(configuration);

let type: string; // (optional) (default to undefined)
let searchKey: string; // (optional) (default to undefined)
let sorting: string; // (optional) (default to undefined)
let skipCount: number; // (optional) (default to undefined)
let maxResultCount: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.getListWithUser(
    type,
    searchKey,
    sorting,
    skipCount,
    maxResultCount
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **type** | [**string**] |  | (optional) defaults to undefined|
| **searchKey** | [**string**] |  | (optional) defaults to undefined|
| **sorting** | [**string**] |  | (optional) defaults to undefined|
| **skipCount** | [**number**] |  | (optional) defaults to undefined|
| **maxResultCount** | [**number**] |  | (optional) defaults to undefined|


### Return type

**AppWithUserDtoPagedResultDto**

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

# **getSdksById**
> Array<AppSdkDto> getSdksById()


### Example

```typescript
import {
    AppApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppApi(configuration);

let appId: string; // (default to undefined)
let env: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getSdksById(
    appId,
    env
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appId** | [**string**] |  | defaults to undefined|
| **env** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Array<AppSdkDto>**

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

# **getUploadCredentials**
> StorageObjectCredentials getUploadCredentials()


### Example

```typescript
import {
    AppApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppApi(configuration);

let key: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getUploadCredentials(
    key
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **key** | [**string**] |  | (optional) defaults to undefined|


### Return type

**StorageObjectCredentials**

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

# **getWithUser**
> AppWithUserDto getWithUser()


### Example

```typescript
import {
    AppApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getWithUser(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AppWithUserDto**

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

# **run**
> AppRunRecordDto run()


### Example

```typescript
import {
    AppApi,
    Configuration,
    AppRunDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppApi(configuration);

let appRunDto: AppRunDto; // (optional)

const { status, data } = await apiInstance.run(
    appRunDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appRunDto** | **AppRunDto**|  | |


### Return type

**AppRunRecordDto**

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

# **updateApp**
> AppDto updateApp()


### Example

```typescript
import {
    AppApi,
    Configuration,
    CreateOrUpdateAppDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppApi(configuration);

let id: string; // (default to undefined)
let createOrUpdateAppDto: CreateOrUpdateAppDto; // (optional)

const { status, data } = await apiInstance.updateApp(
    id,
    createOrUpdateAppDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateAppDto** | **CreateOrUpdateAppDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AppDto**

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

# **updateRunState**
> AppRunRecordDto updateRunState()


### Example

```typescript
import {
    AppApi,
    Configuration,
    AppRunRecordUpdateDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppApi(configuration);

let id: string; // (default to undefined)
let appRunRecordUpdateDto: AppRunRecordUpdateDto; // (optional)

const { status, data } = await apiInstance.updateRunState(
    id,
    appRunRecordUpdateDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appRunRecordUpdateDto** | **AppRunRecordUpdateDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AppRunRecordDto**

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

