# PermissionsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getPermissions**](#getpermissions) | **GET** /api/permission-management/permissions | |
|[**updatePermissions**](#updatepermissions) | **PUT** /api/permission-management/permissions | |

# **getPermissions**
> GetPermissionListResultDto getPermissions()


### Example

```typescript
import {
    PermissionsApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new PermissionsApi(configuration);

let providerName: string; // (optional) (default to undefined)
let providerKey: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getPermissions(
    providerName,
    providerKey
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **providerName** | [**string**] |  | (optional) defaults to undefined|
| **providerKey** | [**string**] |  | (optional) defaults to undefined|


### Return type

**GetPermissionListResultDto**

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

# **updatePermissions**
> updatePermissions()


### Example

```typescript
import {
    PermissionsApi,
    Configuration,
    UpdatePermissionsDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new PermissionsApi(configuration);

let providerName: string; // (optional) (default to undefined)
let providerKey: string; // (optional) (default to undefined)
let updatePermissionsDto: UpdatePermissionsDto; // (optional)

const { status, data } = await apiInstance.updatePermissions(
    providerName,
    providerKey,
    updatePermissionsDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updatePermissionsDto** | **UpdatePermissionsDto**|  | |
| **providerName** | [**string**] |  | (optional) defaults to undefined|
| **providerKey** | [**string**] |  | (optional) defaults to undefined|


### Return type

void (empty response body)

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

