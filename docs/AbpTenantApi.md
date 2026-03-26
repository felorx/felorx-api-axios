# AbpTenantApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**findTenantById**](#findtenantbyid) | **GET** /api/abp/multi-tenancy/tenants/by-id/{id} | |
|[**findTenantByName**](#findtenantbyname) | **GET** /api/abp/multi-tenancy/tenants/by-name/{name} | |

# **findTenantById**
> FindTenantResultDto findTenantById()


### Example

```typescript
import {
    AbpTenantApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AbpTenantApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.findTenantById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**FindTenantResultDto**

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

# **findTenantByName**
> FindTenantResultDto findTenantByName()


### Example

```typescript
import {
    AbpTenantApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AbpTenantApi(configuration);

let name: string; // (default to undefined)

const { status, data } = await apiInstance.findTenantByName(
    name
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **name** | [**string**] |  | defaults to undefined|


### Return type

**FindTenantResultDto**

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

