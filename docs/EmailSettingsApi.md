# EmailSettingsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getEmailSettings**](#getemailsettings) | **GET** /api/setting-management/emailing | |
|[**sendTestEmail**](#sendtestemail) | **POST** /api/setting-management/emailing/send-test-email | |
|[**updateEmailSettings**](#updateemailsettings) | **POST** /api/setting-management/emailing | |

# **getEmailSettings**
> EmailSettingsDto getEmailSettings()


### Example

```typescript
import {
    EmailSettingsApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new EmailSettingsApi(configuration);

const { status, data } = await apiInstance.getEmailSettings();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**EmailSettingsDto**

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

# **sendTestEmail**
> sendTestEmail()


### Example

```typescript
import {
    EmailSettingsApi,
    Configuration,
    SendTestEmailInput
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new EmailSettingsApi(configuration);

let sendTestEmailInput: SendTestEmailInput; // (optional)

const { status, data } = await apiInstance.sendTestEmail(
    sendTestEmailInput
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sendTestEmailInput** | **SendTestEmailInput**|  | |


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

# **updateEmailSettings**
> updateEmailSettings()


### Example

```typescript
import {
    EmailSettingsApi,
    Configuration,
    UpdateEmailSettingsDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new EmailSettingsApi(configuration);

let updateEmailSettingsDto: UpdateEmailSettingsDto; // (optional)

const { status, data } = await apiInstance.updateEmailSettings(
    updateEmailSettingsDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **updateEmailSettingsDto** | **UpdateEmailSettingsDto**|  | |


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

