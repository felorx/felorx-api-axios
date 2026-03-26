# MessageApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**publish**](#publish) | **POST** /api/app/message/publish | |
|[**recall**](#recall) | **POST** /api/app/message/recall | |
|[**subscribe**](#subscribe) | **POST** /api/app/message/subscribe | |
|[**unsubscribe**](#unsubscribe) | **POST** /api/app/message/unsubscribe | |

# **publish**
> publish()


### Example

```typescript
import {
    MessageApi,
    Configuration,
    MessagePublishDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageApi(configuration);

let messagePublishDto: MessagePublishDto; // (optional)

const { status, data } = await apiInstance.publish(
    messagePublishDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **messagePublishDto** | **MessagePublishDto**|  | |


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

# **recall**
> recall()


### Example

```typescript
import {
    MessageApi,
    Configuration,
    MessageRecallDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageApi(configuration);

let messageRecallDto: MessageRecallDto; // (optional)

const { status, data } = await apiInstance.recall(
    messageRecallDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **messageRecallDto** | **MessageRecallDto**|  | |


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

# **subscribe**
> subscribe()


### Example

```typescript
import {
    MessageApi,
    Configuration,
    MessageSubscribeDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageApi(configuration);

let messageSubscribeDto: MessageSubscribeDto; // (optional)

const { status, data } = await apiInstance.subscribe(
    messageSubscribeDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **messageSubscribeDto** | **MessageSubscribeDto**|  | |


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

# **unsubscribe**
> unsubscribe()


### Example

```typescript
import {
    MessageApi,
    Configuration,
    MessageUnsubscribeDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageApi(configuration);

let messageUnsubscribeDto: MessageUnsubscribeDto; // (optional)

const { status, data } = await apiInstance.unsubscribe(
    messageUnsubscribeDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **messageUnsubscribeDto** | **MessageUnsubscribeDto**|  | |


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

