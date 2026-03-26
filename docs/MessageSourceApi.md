# MessageSourceApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createMessageSource**](#createmessagesource) | **POST** /api/app/message-source | |
|[**deleteMessageSourceById**](#deletemessagesourcebyid) | **DELETE** /api/app/message-source/{id} | |
|[**getMessageSourceById**](#getmessagesourcebyid) | **GET** /api/app/message-source/{id} | |
|[**getMessageSourceList**](#getmessagesourcelist) | **GET** /api/app/message-source | |
|[**updateMessageSource**](#updatemessagesource) | **PUT** /api/app/message-source/{id} | |

# **createMessageSource**
> CreateUpdateMessageSourceDto createMessageSource()


### Example

```typescript
import {
    MessageSourceApi,
    Configuration,
    CreateUpdateMessageSourceDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageSourceApi(configuration);

let createUpdateMessageSourceDto: CreateUpdateMessageSourceDto; // (optional)

const { status, data } = await apiInstance.createMessageSource(
    createUpdateMessageSourceDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createUpdateMessageSourceDto** | **CreateUpdateMessageSourceDto**|  | |


### Return type

**CreateUpdateMessageSourceDto**

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

# **deleteMessageSourceById**
> deleteMessageSourceById()


### Example

```typescript
import {
    MessageSourceApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageSourceApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteMessageSourceById(
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

# **getMessageSourceById**
> MessageSourceDto getMessageSourceById()


### Example

```typescript
import {
    MessageSourceApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageSourceApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getMessageSourceById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**MessageSourceDto**

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

# **getMessageSourceList**
> Array<MessageSourceDto> getMessageSourceList()


### Example

```typescript
import {
    MessageSourceApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageSourceApi(configuration);

let categoryId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getMessageSourceList(
    categoryId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **categoryId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Array<MessageSourceDto>**

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

# **updateMessageSource**
> CreateUpdateMessageSourceDto updateMessageSource()


### Example

```typescript
import {
    MessageSourceApi,
    Configuration,
    CreateUpdateMessageSourceDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageSourceApi(configuration);

let id: string; // (default to undefined)
let createUpdateMessageSourceDto: CreateUpdateMessageSourceDto; // (optional)

const { status, data } = await apiInstance.updateMessageSource(
    id,
    createUpdateMessageSourceDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createUpdateMessageSourceDto** | **CreateUpdateMessageSourceDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**CreateUpdateMessageSourceDto**

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

