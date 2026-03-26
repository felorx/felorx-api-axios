# ProfileApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**changePassword**](#changepassword) | **POST** /api/account/my-profile/change-password | |
|[**getProfile**](#getprofile) | **GET** /api/account/my-profile | |
|[**updateProfile**](#updateprofile) | **PUT** /api/account/my-profile | |

# **changePassword**
> changePassword()


### Example

```typescript
import {
    ProfileApi,
    Configuration,
    ChangePasswordInput
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new ProfileApi(configuration);

let changePasswordInput: ChangePasswordInput; // (optional)

const { status, data } = await apiInstance.changePassword(
    changePasswordInput
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **changePasswordInput** | **ChangePasswordInput**|  | |


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

# **getProfile**
> ProfileDto getProfile()


### Example

```typescript
import {
    ProfileApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new ProfileApi(configuration);

const { status, data } = await apiInstance.getProfile();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**ProfileDto**

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

# **updateProfile**
> ProfileDto updateProfile()


### Example

```typescript
import {
    ProfileApi,
    Configuration,
    UpdateProfileDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new ProfileApi(configuration);

let updateProfileDto: UpdateProfileDto; // (optional)

const { status, data } = await apiInstance.updateProfile(
    updateProfileDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateProfileDto** | **UpdateProfileDto**|  | |


### Return type

**ProfileDto**

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

