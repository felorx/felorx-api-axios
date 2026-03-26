# MessageSourceRouteSubApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createMessageSourceRouteSub**](#createmessagesourceroutesub) | **POST** /api/app/message-source-route-sub | |
|[**deleteMessageSourceRouteSubById**](#deletemessagesourceroutesubbyid) | **DELETE** /api/app/message-source-route-sub/{id} | |
|[**getMessageSourceRouteSubById**](#getmessagesourceroutesubbyid) | **GET** /api/app/message-source-route-sub/{id} | |
|[**getMessageSourceRouteSubList**](#getmessagesourceroutesublist) | **GET** /api/app/message-source-route-sub | |
|[**updateMessageSourceRouteSub**](#updatemessagesourceroutesub) | **PUT** /api/app/message-source-route-sub/{id} | |

# **createMessageSourceRouteSub**
> createMessageSourceRouteSub()


### Example

```typescript
import {
    MessageSourceRouteSubApi,
    Configuration,
    CreateUpdateMessageSourceRouteSubDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageSourceRouteSubApi(configuration);

let createUpdateMessageSourceRouteSubDto: CreateUpdateMessageSourceRouteSubDto; // (optional)

const { status, data } = await apiInstance.createMessageSourceRouteSub(
    createUpdateMessageSourceRouteSubDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createUpdateMessageSourceRouteSubDto** | **CreateUpdateMessageSourceRouteSubDto**|  | |


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

# **deleteMessageSourceRouteSubById**
> deleteMessageSourceRouteSubById()


### Example

```typescript
import {
    MessageSourceRouteSubApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageSourceRouteSubApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteMessageSourceRouteSubById(
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

# **getMessageSourceRouteSubById**
> MessageSourceRouteSubDto getMessageSourceRouteSubById()


### Example

```typescript
import {
    MessageSourceRouteSubApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageSourceRouteSubApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getMessageSourceRouteSubById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**MessageSourceRouteSubDto**

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

# **getMessageSourceRouteSubList**
> Array<MessageSourceRouteSubDto> getMessageSourceRouteSubList()


### Example

```typescript
import {
    MessageSourceRouteSubApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageSourceRouteSubApi(configuration);

const { status, data } = await apiInstance.getMessageSourceRouteSubList();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<MessageSourceRouteSubDto>**

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

# **updateMessageSourceRouteSub**
> updateMessageSourceRouteSub()


### Example

```typescript
import {
    MessageSourceRouteSubApi,
    Configuration,
    CreateUpdateMessageSourceRouteSubDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageSourceRouteSubApi(configuration);

let id: string; // (default to undefined)
let createUpdateMessageSourceRouteSubDto: CreateUpdateMessageSourceRouteSubDto; // (optional)

const { status, data } = await apiInstance.updateMessageSourceRouteSub(
    id,
    createUpdateMessageSourceRouteSubDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createUpdateMessageSourceRouteSubDto** | **CreateUpdateMessageSourceRouteSubDto**|  | |
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

