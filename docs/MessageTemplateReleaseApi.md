# MessageTemplateReleaseApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createMessageTemplateRelease**](#createmessagetemplaterelease) | **POST** /api/app/message-template-release | |
|[**getMessageTemplateReleaseById**](#getmessagetemplatereleasebyid) | **GET** /api/app/message-template-release/{id} | |
|[**getMessageTemplateReleaseList**](#getmessagetemplatereleaselist) | **GET** /api/app/message-template-release | |

# **createMessageTemplateRelease**
> MessageTemplateReleaseDto createMessageTemplateRelease()


### Example

```typescript
import {
    MessageTemplateReleaseApi,
    Configuration,
    CreateMessageTemplateReleaseDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageTemplateReleaseApi(configuration);

let createMessageTemplateReleaseDto: CreateMessageTemplateReleaseDto; // (optional)

const { status, data } = await apiInstance.createMessageTemplateRelease(
    createMessageTemplateReleaseDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createMessageTemplateReleaseDto** | **CreateMessageTemplateReleaseDto**|  | |


### Return type

**MessageTemplateReleaseDto**

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

# **getMessageTemplateReleaseById**
> MessageTemplateReleaseDto getMessageTemplateReleaseById()


### Example

```typescript
import {
    MessageTemplateReleaseApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageTemplateReleaseApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getMessageTemplateReleaseById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**MessageTemplateReleaseDto**

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

# **getMessageTemplateReleaseList**
> Array<MessageTemplateReleaseDto> getMessageTemplateReleaseList()


### Example

```typescript
import {
    MessageTemplateReleaseApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageTemplateReleaseApi(configuration);

let templateId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getMessageTemplateReleaseList(
    templateId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **templateId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Array<MessageTemplateReleaseDto>**

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

