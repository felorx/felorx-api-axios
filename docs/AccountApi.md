# AccountApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**changeAccountPassword**](#changeaccountpassword) | **POST** /api/app/account/change-password | |
|[**checkSyncAuth**](#checksyncauth) | **POST** /api/app/account/check-sync-auth | 检查同步认证|
|[**destroyAccount**](#destroyaccount) | **POST** /api/app/account/destroy-account | |
|[**getAccount**](#getaccount) | **GET** /api/app/account | |
|[**register**](#register) | **POST** /api/account/register | |
|[**resetPassword**](#resetpassword) | **POST** /api/account/reset-password | |
|[**sendPasswordResetCode**](#sendpasswordresetcode) | **POST** /api/account/send-password-reset-code | |
|[**verifyPasswordResetToken**](#verifypasswordresettoken) | **POST** /api/account/verify-password-reset-token | |

# **changeAccountPassword**
> changeAccountPassword()


### Example

```typescript
import {
    AccountApi,
    Configuration,
    ChangePasswordDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AccountApi(configuration);

let changePasswordDto: ChangePasswordDto; // (optional)

const { status, data } = await apiInstance.changeAccountPassword(
    changePasswordDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **changePasswordDto** | **ChangePasswordDto**|  | |


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

# **checkSyncAuth**
> CheckSyncAuthResultDto checkSyncAuth()


### Example

```typescript
import {
    AccountApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AccountApi(configuration);

const { status, data } = await apiInstance.checkSyncAuth();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**CheckSyncAuthResultDto**

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

# **destroyAccount**
> destroyAccount()


### Example

```typescript
import {
    AccountApi,
    Configuration,
    AccountDeletionDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AccountApi(configuration);

let accountDeletionDto: AccountDeletionDto; // (optional)

const { status, data } = await apiInstance.destroyAccount(
    accountDeletionDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **accountDeletionDto** | **AccountDeletionDto**|  | |


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

# **getAccount**
> UserProfileDto getAccount()


### Example

```typescript
import {
    AccountApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AccountApi(configuration);

const { status, data } = await apiInstance.getAccount();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**UserProfileDto**

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

# **register**
> IdentityUserDto register()


### Example

```typescript
import {
    AccountApi,
    Configuration,
    RegisterDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AccountApi(configuration);

let registerDto: RegisterDto; // (optional)

const { status, data } = await apiInstance.register(
    registerDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **registerDto** | **RegisterDto**|  | |


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

# **resetPassword**
> resetPassword()


### Example

```typescript
import {
    AccountApi,
    Configuration,
    ResetPasswordDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AccountApi(configuration);

let resetPasswordDto: ResetPasswordDto; // (optional)

const { status, data } = await apiInstance.resetPassword(
    resetPasswordDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **resetPasswordDto** | **ResetPasswordDto**|  | |


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

# **sendPasswordResetCode**
> sendPasswordResetCode()


### Example

```typescript
import {
    AccountApi,
    Configuration,
    SendPasswordResetCodeDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AccountApi(configuration);

let sendPasswordResetCodeDto: SendPasswordResetCodeDto; // (optional)

const { status, data } = await apiInstance.sendPasswordResetCode(
    sendPasswordResetCodeDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sendPasswordResetCodeDto** | **SendPasswordResetCodeDto**|  | |


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

# **verifyPasswordResetToken**
> boolean verifyPasswordResetToken()


### Example

```typescript
import {
    AccountApi,
    Configuration,
    VerifyPasswordResetTokenInput
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AccountApi(configuration);

let verifyPasswordResetTokenInput: VerifyPasswordResetTokenInput; // (optional)

const { status, data } = await apiInstance.verifyPasswordResetToken(
    verifyPasswordResetTokenInput
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **verifyPasswordResetTokenInput** | **VerifyPasswordResetTokenInput**|  | |


### Return type

**boolean**

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

