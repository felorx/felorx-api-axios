# ApiKeysApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createApiKeys**](#createapikeys) | **POST** /api/api-keys | |
|[**deleteApiKeysById**](#deleteapikeysbyid) | **DELETE** /api/api-keys/{id} | |
|[**getApiKeysById**](#getapikeysbyid) | **GET** /api/api-keys/{id} | |
|[**getApiKeysList**](#getapikeyslist) | **GET** /api/api-keys | |
|[**updateApiKeys**](#updateapikeys) | **PUT** /api/api-keys/{id} | |

# **createApiKeys**
> ApiKeyDto createApiKeys()


### Example

```typescript
import {
    ApiKeysApi,
    Configuration,
    ApiKeyCreateDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new ApiKeysApi(configuration);

let apiKeyCreateDto: ApiKeyCreateDto; // (optional)

const { status, data } = await apiInstance.createApiKeys(
    apiKeyCreateDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **apiKeyCreateDto** | **ApiKeyCreateDto**|  | |


### Return type

**ApiKeyDto**

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

# **deleteApiKeysById**
> deleteApiKeysById()


### Example

```typescript
import {
    ApiKeysApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new ApiKeysApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteApiKeysById(
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

# **getApiKeysById**
> ApiKeyDto getApiKeysById()


### Example

```typescript
import {
    ApiKeysApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new ApiKeysApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getApiKeysById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**ApiKeyDto**

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

# **getApiKeysList**
> ApiKeyDtoPagedResultDto getApiKeysList()


### Example

```typescript
import {
    ApiKeysApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new ApiKeysApi(configuration);

let sorting: string; // (optional) (default to undefined)
let skipCount: number; // (optional) (default to undefined)
let maxResultCount: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.getApiKeysList(
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

**ApiKeyDtoPagedResultDto**

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

# **updateApiKeys**
> ApiKeyDto updateApiKeys()


### Example

```typescript
import {
    ApiKeysApi,
    Configuration,
    ApiKeyUpdateDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new ApiKeysApi(configuration);

let id: string; // (default to undefined)
let apiKeyUpdateDto: ApiKeyUpdateDto; // (optional)

const { status, data } = await apiInstance.updateApiKeys(
    id,
    apiKeyUpdateDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **apiKeyUpdateDto** | **ApiKeyUpdateDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**ApiKeyDto**

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

