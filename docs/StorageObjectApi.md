# StorageObjectApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getCdnDomains**](#getcdndomains) | **GET** /api/app/storage-object/cdn-domains | 获取所有 CDN Domain 配置|
|[**getFileCredential**](#getfilecredential) | **GET** /api/app/storage-object/file-credential | |
|[**getUserStorages**](#getuserstorages) | **GET** /api/app/storage-object/user-storages | |
|[**preSignUrl**](#presignurl) | **POST** /api/app/storage-object/pre-sign-url | |

# **getCdnDomains**
> Array<CdnDomainDto> getCdnDomains()


### Example

```typescript
import {
    StorageObjectApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new StorageObjectApi(configuration);

const { status, data } = await apiInstance.getCdnDomains();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<CdnDomainDto>**

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

# **getFileCredential**
> StorageObjectCredentials getFileCredential()


### Example

```typescript
import {
    StorageObjectApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new StorageObjectApi(configuration);

let userTotalSize: number; // (optional) (default to undefined)
let rapidCode: string; // (optional) (default to undefined)
let usage: string; // (optional) (default to undefined)
let key: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getFileCredential(
    userTotalSize,
    rapidCode,
    usage,
    key
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userTotalSize** | [**number**] |  | (optional) defaults to undefined|
| **rapidCode** | [**string**] |  | (optional) defaults to undefined|
| **usage** | [**string**] |  | (optional) defaults to undefined|
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

# **getUserStorages**
> Array<UserStorageDto> getUserStorages()


### Example

```typescript
import {
    StorageObjectApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new StorageObjectApi(configuration);

const { status, data } = await apiInstance.getUserStorages();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<UserStorageDto>**

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

# **preSignUrl**
> string preSignUrl()


### Example

```typescript
import {
    StorageObjectApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new StorageObjectApi(configuration);

let bucket: string; // (optional) (default to undefined)
let key: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.preSignUrl(
    bucket,
    key
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **bucket** | [**string**] |  | (optional) defaults to undefined|
| **key** | [**string**] |  | (optional) defaults to undefined|


### Return type

**string**

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

