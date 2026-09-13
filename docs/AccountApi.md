# AccountApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**changeAccountPassword**](#changeaccountpassword) | **POST** /api/app/account/change-password | |
|[**checkSyncAuth**](#checksyncauth) | **POST** /api/app/account/check-sync-auth | 检查同步认证|
|[**deletionStatus**](#deletionstatus) | **POST** /api/app/account/deletion-status | |
|[**destroyAccount**](#destroyaccount) | **POST** /api/app/account/destroy-account | |
|[**getAccountGetApiAppAccount**](#getaccountgetapiappaccount) | **GET** /api/app/account | |
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
} from 'felorx-api';

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

No authorization required

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
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AccountApi(configuration);

const { status, data } = await apiInstance.checkSyncAuth();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**CheckSyncAuthResultDto**

### Authorization

No authorization required

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

# **deletionStatus**
> AccountDeletionStatusDto deletionStatus()


### Example

```typescript
import {
    AccountApi,
    Configuration,
    AccountDeletionStatusQueryDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AccountApi(configuration);

let accountDeletionStatusQueryDto: AccountDeletionStatusQueryDto; // (optional)

const { status, data } = await apiInstance.deletionStatus(
    accountDeletionStatusQueryDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **accountDeletionStatusQueryDto** | **AccountDeletionStatusQueryDto**|  | |


### Return type

**AccountDeletionStatusDto**

### Authorization

No authorization required

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

# **destroyAccount**
> AccountDeletionStatusDto destroyAccount()


### Example

```typescript
import {
    AccountApi,
    Configuration,
    AccountDeletionDto
} from 'felorx-api';

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

**AccountDeletionStatusDto**

### Authorization

No authorization required

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

# **getAccountGetApiAppAccount**
> UserProfileDto getAccountGetApiAppAccount()


### Example

```typescript
import {
    AccountApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AccountApi(configuration);

const { status, data } = await apiInstance.getAccountGetApiAppAccount();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**UserProfileDto**

### Authorization

No authorization required

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
} from 'felorx-api';

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

No authorization required

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
} from 'felorx-api';

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

No authorization required

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
} from 'felorx-api';

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

No authorization required

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
} from 'felorx-api';

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

No authorization required

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

