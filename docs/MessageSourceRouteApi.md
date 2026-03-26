# MessageSourceRouteApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createMessageSourceRoute**](#createmessagesourceroute) | **POST** /api/app/message-source-route | |
|[**deleteMessageSourceRouteById**](#deletemessagesourceroutebyid) | **DELETE** /api/app/message-source-route/{id} | |
|[**getMessageSourceRouteById**](#getmessagesourceroutebyid) | **GET** /api/app/message-source-route/{id} | |
|[**getMessageSourceRouteList**](#getmessagesourceroutelist) | **GET** /api/app/message-source-route | |
|[**updateMessageSourceRoute**](#updatemessagesourceroute) | **PUT** /api/app/message-source-route/{id} | |

# **createMessageSourceRoute**
> createMessageSourceRoute()


### Example

```typescript
import {
    MessageSourceRouteApi,
    Configuration,
    CreateUpdateMessageSourceRouteDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageSourceRouteApi(configuration);

let createUpdateMessageSourceRouteDto: CreateUpdateMessageSourceRouteDto; // (optional)

const { status, data } = await apiInstance.createMessageSourceRoute(
    createUpdateMessageSourceRouteDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createUpdateMessageSourceRouteDto** | **CreateUpdateMessageSourceRouteDto**|  | |


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

# **deleteMessageSourceRouteById**
> deleteMessageSourceRouteById()


### Example

```typescript
import {
    MessageSourceRouteApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageSourceRouteApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteMessageSourceRouteById(
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

# **getMessageSourceRouteById**
> MessageSourceRouteDto getMessageSourceRouteById()


### Example

```typescript
import {
    MessageSourceRouteApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageSourceRouteApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getMessageSourceRouteById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**MessageSourceRouteDto**

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

# **getMessageSourceRouteList**
> Array<MessageSourceRouteDto> getMessageSourceRouteList()


### Example

```typescript
import {
    MessageSourceRouteApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageSourceRouteApi(configuration);

let sourceId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getMessageSourceRouteList(
    sourceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sourceId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**Array<MessageSourceRouteDto>**

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

# **updateMessageSourceRoute**
> updateMessageSourceRoute()


### Example

```typescript
import {
    MessageSourceRouteApi,
    Configuration,
    CreateUpdateMessageSourceRouteDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageSourceRouteApi(configuration);

let id: string; // (default to undefined)
let createUpdateMessageSourceRouteDto: CreateUpdateMessageSourceRouteDto; // (optional)

const { status, data } = await apiInstance.updateMessageSourceRoute(
    id,
    createUpdateMessageSourceRouteDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createUpdateMessageSourceRouteDto** | **CreateUpdateMessageSourceRouteDto**|  | |
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

