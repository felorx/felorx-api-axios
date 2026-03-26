# MessageTemplateApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createMessageTemplate**](#createmessagetemplate) | **POST** /api/app/message-template | |
|[**deleteMessageTemplateById**](#deletemessagetemplatebyid) | **DELETE** /api/app/message-template/{id} | |
|[**getMessageTemplateById**](#getmessagetemplatebyid) | **GET** /api/app/message-template/{id} | |
|[**getMessageTemplateList**](#getmessagetemplatelist) | **GET** /api/app/message-template | |
|[**updateMessageTemplate**](#updatemessagetemplate) | **PUT** /api/app/message-template/{id} | |

# **createMessageTemplate**
> MessageTemplateDto createMessageTemplate()


### Example

```typescript
import {
    MessageTemplateApi,
    Configuration,
    CreateOrUpdateMessageTemplateDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageTemplateApi(configuration);

let createOrUpdateMessageTemplateDto: CreateOrUpdateMessageTemplateDto; // (optional)

const { status, data } = await apiInstance.createMessageTemplate(
    createOrUpdateMessageTemplateDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateMessageTemplateDto** | **CreateOrUpdateMessageTemplateDto**|  | |


### Return type

**MessageTemplateDto**

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

# **deleteMessageTemplateById**
> deleteMessageTemplateById()


### Example

```typescript
import {
    MessageTemplateApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageTemplateApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteMessageTemplateById(
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

# **getMessageTemplateById**
> MessageTemplateDto getMessageTemplateById()


### Example

```typescript
import {
    MessageTemplateApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageTemplateApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getMessageTemplateById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**MessageTemplateDto**

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

# **getMessageTemplateList**
> Array<MessageTemplateDto> getMessageTemplateList()


### Example

```typescript
import {
    MessageTemplateApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageTemplateApi(configuration);

const { status, data } = await apiInstance.getMessageTemplateList();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<MessageTemplateDto>**

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

# **updateMessageTemplate**
> MessageTemplateDto updateMessageTemplate()


### Example

```typescript
import {
    MessageTemplateApi,
    Configuration,
    CreateOrUpdateMessageTemplateDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageTemplateApi(configuration);

let id: string; // (default to undefined)
let createOrUpdateMessageTemplateDto: CreateOrUpdateMessageTemplateDto; // (optional)

const { status, data } = await apiInstance.updateMessageTemplate(
    id,
    createOrUpdateMessageTemplateDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateMessageTemplateDto** | **CreateOrUpdateMessageTemplateDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**MessageTemplateDto**

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

