# UserApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createIdentityUser**](#createidentityuser) | **POST** /api/identity/users | |
|[**deleteIdentityUserById**](#deleteidentityuserbyid) | **DELETE** /api/identity/users/{id} | |
|[**findByEmail**](#findbyemail) | **GET** /api/identity/users/by-email/{email} | |
|[**findByUsername**](#findbyusername) | **GET** /api/identity/users/by-username/{userName} | |
|[**getAssignableRoles**](#getassignableroles) | **GET** /api/identity/users/assignable-roles | |
|[**getIdentityUserById**](#getidentityuserbyid) | **GET** /api/identity/users/{id} | |
|[**getIdentityUserList**](#getidentityuserlist) | **GET** /api/identity/users | |
|[**getRoles**](#getroles) | **GET** /api/identity/users/{id}/roles | |
|[**updateIdentityUser**](#updateidentityuser) | **PUT** /api/identity/users/{id} | |
|[**updateRoles**](#updateroles) | **PUT** /api/identity/users/{id}/roles | |

# **createIdentityUser**
> IdentityUserDto createIdentityUser()


### Example

```typescript
import {
    UserApi,
    Configuration,
    IdentityUserCreateDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let identityUserCreateDto: IdentityUserCreateDto; // (optional)

const { status, data } = await apiInstance.createIdentityUser(
    identityUserCreateDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **identityUserCreateDto** | **IdentityUserCreateDto**|  | |


### Return type

**IdentityUserDto**

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

# **deleteIdentityUserById**
> deleteIdentityUserById()


### Example

```typescript
import {
    UserApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteIdentityUserById(
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

# **findByEmail**
> IdentityUserDto findByEmail()


### Example

```typescript
import {
    UserApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let email: string; // (default to undefined)

const { status, data } = await apiInstance.findByEmail(
    email
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **email** | [**string**] |  | defaults to undefined|


### Return type

**IdentityUserDto**

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

# **findByUsername**
> IdentityUserDto findByUsername()


### Example

```typescript
import {
    UserApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let userName: string; // (default to undefined)

const { status, data } = await apiInstance.findByUsername(
    userName
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userName** | [**string**] |  | defaults to undefined|


### Return type

**IdentityUserDto**

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

# **getAssignableRoles**
> IdentityRoleDtoListResultDto getAssignableRoles()


### Example

```typescript
import {
    UserApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

const { status, data } = await apiInstance.getAssignableRoles();
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

# **getIdentityUserById**
> IdentityUserDto getIdentityUserById()


### Example

```typescript
import {
    UserApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getIdentityUserById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**IdentityUserDto**

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

# **getIdentityUserList**
> IdentityUserDtoPagedResultDto getIdentityUserList()


### Example

```typescript
import {
    UserApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let filter: string; // (optional) (default to undefined)
let sorting: string; // (optional) (default to undefined)
let skipCount: number; // (optional) (default to undefined)
let maxResultCount: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.getIdentityUserList(
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

**IdentityUserDtoPagedResultDto**

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

# **getRoles**
> IdentityRoleDtoListResultDto getRoles()


### Example

```typescript
import {
    UserApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getRoles(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


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

# **updateIdentityUser**
> IdentityUserDto updateIdentityUser()


### Example

```typescript
import {
    UserApi,
    Configuration,
    IdentityUserUpdateDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let id: string; // (default to undefined)
let identityUserUpdateDto: IdentityUserUpdateDto; // (optional)

const { status, data } = await apiInstance.updateIdentityUser(
    id,
    identityUserUpdateDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **identityUserUpdateDto** | **IdentityUserUpdateDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**IdentityUserDto**

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

# **updateRoles**
> updateRoles()


### Example

```typescript
import {
    UserApi,
    Configuration,
    IdentityUserUpdateRolesDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new UserApi(configuration);

let id: string; // (default to undefined)
let identityUserUpdateRolesDto: IdentityUserUpdateRolesDto; // (optional)

const { status, data } = await apiInstance.updateRoles(
    id,
    identityUserUpdateRolesDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **identityUserUpdateRolesDto** | **IdentityUserUpdateRolesDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


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

