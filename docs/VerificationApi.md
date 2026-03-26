# VerificationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**sendCode**](#sendcode) | **POST** /api/app/verification/send-code | |
|[**sendCodeAnonymous**](#sendcodeanonymous) | **POST** /api/app/verification/send-code-anonymous | |

# **sendCode**
> sendCode()


### Example

```typescript
import {
    VerificationApi,
    Configuration,
    SendVerificationCodeDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new VerificationApi(configuration);

let sendVerificationCodeDto: SendVerificationCodeDto; // (optional)

const { status, data } = await apiInstance.sendCode(
    sendVerificationCodeDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sendVerificationCodeDto** | **SendVerificationCodeDto**|  | |


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

# **sendCodeAnonymous**
> sendCodeAnonymous()


### Example

```typescript
import {
    VerificationApi,
    Configuration,
    SendVerificationCodeDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new VerificationApi(configuration);

let sendVerificationCodeDto: SendVerificationCodeDto; // (optional)

const { status, data } = await apiInstance.sendCodeAnonymous(
    sendVerificationCodeDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sendVerificationCodeDto** | **SendVerificationCodeDto**|  | |


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

