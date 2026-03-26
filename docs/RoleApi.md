# RoleApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createIdentityRole**](#createidentityrole) | **POST** /api/identity/roles | |
|[**deleteIdentityRoleById**](#deleteidentityrolebyid) | **DELETE** /api/identity/roles/{id} | |
|[**getAllList**](#getalllist) | **GET** /api/identity/roles/all | |
|[**getIdentityRoleById**](#getidentityrolebyid) | **GET** /api/identity/roles/{id} | |
|[**getIdentityRoleList**](#getidentityrolelist) | **GET** /api/identity/roles | |
|[**updateIdentityRole**](#updateidentityrole) | **PUT** /api/identity/roles/{id} | |

# **createIdentityRole**
> IdentityRoleDto createIdentityRole()


### Example

```typescript
import {
    RoleApi,
    Configuration,
    IdentityRoleCreateDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new RoleApi(configuration);

let identityRoleCreateDto: IdentityRoleCreateDto; // (optional)

const { status, data } = await apiInstance.createIdentityRole(
    identityRoleCreateDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **identityRoleCreateDto** | **IdentityRoleCreateDto**|  | |


### Return type

**IdentityRoleDto**

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

# **deleteIdentityRoleById**
> deleteIdentityRoleById()


### Example

```typescript
import {
    RoleApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new RoleApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteIdentityRoleById(
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

# **getAllList**
> IdentityRoleDtoListResultDto getAllList()


### Example

```typescript
import {
    RoleApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new RoleApi(configuration);

const { status, data } = await apiInstance.getAllList();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**IdentityRoleDtoListResultDto**

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

# **getIdentityRoleById**
> IdentityRoleDto getIdentityRoleById()


### Example

```typescript
import {
    RoleApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new RoleApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getIdentityRoleById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**IdentityRoleDto**

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

# **getIdentityRoleList**
> IdentityRoleDtoPagedResultDto getIdentityRoleList()


### Example

```typescript
import {
    RoleApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new RoleApi(configuration);

let filter: string; // (optional) (default to undefined)
let sorting: string; // (optional) (default to undefined)
let skipCount: number; // (optional) (default to undefined)
let maxResultCount: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.getIdentityRoleList(
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

**IdentityRoleDtoPagedResultDto**

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

# **updateIdentityRole**
> IdentityRoleDto updateIdentityRole()


### Example

```typescript
import {
    RoleApi,
    Configuration,
    IdentityRoleUpdateDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new RoleApi(configuration);

let id: string; // (default to undefined)
let identityRoleUpdateDto: IdentityRoleUpdateDto; // (optional)

const { status, data } = await apiInstance.updateIdentityRole(
    id,
    identityRoleUpdateDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **identityRoleUpdateDto** | **IdentityRoleUpdateDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**IdentityRoleDto**

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

