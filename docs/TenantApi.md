# TenantApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createTenant**](#createtenant) | **POST** /api/multi-tenancy/tenants | |
|[**deleteDefaultConnectionString**](#deletedefaultconnectionstring) | **DELETE** /api/multi-tenancy/tenants/{id}/default-connection-string | |
|[**deleteTenantById**](#deletetenantbyid) | **DELETE** /api/multi-tenancy/tenants/{id} | |
|[**getDefaultConnectionString**](#getdefaultconnectionstring) | **GET** /api/multi-tenancy/tenants/{id}/default-connection-string | |
|[**getTenantById**](#gettenantbyid) | **GET** /api/multi-tenancy/tenants/{id} | |
|[**getTenantList**](#gettenantlist) | **GET** /api/multi-tenancy/tenants | |
|[**updateDefaultConnectionString**](#updatedefaultconnectionstring) | **PUT** /api/multi-tenancy/tenants/{id}/default-connection-string | |
|[**updateTenant**](#updatetenant) | **PUT** /api/multi-tenancy/tenants/{id} | |

# **createTenant**
> TenantDto createTenant()


### Example

```typescript
import {
    TenantApi,
    Configuration,
    TenantCreateDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new TenantApi(configuration);

let tenantCreateDto: TenantCreateDto; // (optional)

const { status, data } = await apiInstance.createTenant(
    tenantCreateDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tenantCreateDto** | **TenantCreateDto**|  | |


### Return type

**TenantDto**

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

# **deleteDefaultConnectionString**
> deleteDefaultConnectionString()


### Example

```typescript
import {
    TenantApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new TenantApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteDefaultConnectionString(
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

# **deleteTenantById**
> deleteTenantById()


### Example

```typescript
import {
    TenantApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new TenantApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteTenantById(
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

# **getDefaultConnectionString**
> string getDefaultConnectionString()


### Example

```typescript
import {
    TenantApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new TenantApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getDefaultConnectionString(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


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

# **getTenantById**
> TenantDto getTenantById()


### Example

```typescript
import {
    TenantApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new TenantApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getTenantById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**TenantDto**

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

# **getTenantList**
> TenantDtoPagedResultDto getTenantList()


### Example

```typescript
import {
    TenantApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new TenantApi(configuration);

let filter: string; // (optional) (default to undefined)
let sorting: string; // (optional) (default to undefined)
let skipCount: number; // (optional) (default to undefined)
let maxResultCount: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.getTenantList(
    filter,
    sorting,
    skipCount,
    maxResultCount
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **filter** | [**string**] |  | (optional) defaults to undefined|
| **sorting** | [**string**] |  | (optional) defaults to undefined|
| **skipCount** | [**number**] |  | (optional) defaults to undefined|
| **maxResultCount** | [**number**] |  | (optional) defaults to undefined|


### Return type

**TenantDtoPagedResultDto**

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

# **updateDefaultConnectionString**
> updateDefaultConnectionString()


### Example

```typescript
import {
    TenantApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new TenantApi(configuration);

let id: string; // (default to undefined)
let defaultConnectionString: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateDefaultConnectionString(
    id,
    defaultConnectionString
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **defaultConnectionString** | [**string**] |  | (optional) defaults to undefined|


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

# **updateTenant**
> TenantDto updateTenant()


### Example

```typescript
import {
    TenantApi,
    Configuration,
    TenantUpdateDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new TenantApi(configuration);

let id: string; // (default to undefined)
let tenantUpdateDto: TenantUpdateDto; // (optional)

const { status, data } = await apiInstance.updateTenant(
    id,
    tenantUpdateDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **tenantUpdateDto** | **TenantUpdateDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**TenantDto**

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

