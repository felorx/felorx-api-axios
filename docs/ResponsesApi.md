# ResponsesApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**cancelResponse**](#cancelresponse) | **POST** /api/ai/v1/responses/{id}/cancel | |
|[**cancelResponseLegacy**](#cancelresponselegacy) | **POST** /api/ai/openai/responses/{id}/cancel | |
|[**compactResponse**](#compactresponse) | **POST** /api/ai/v1/responses/compact | |
|[**compactResponseLegacy**](#compactresponselegacy) | **POST** /api/ai/openai/responses/compact | |
|[**countResponseInputTokens**](#countresponseinputtokens) | **POST** /api/ai/v1/responses/input_tokens | |
|[**countResponseInputTokensLegacy**](#countresponseinputtokenslegacy) | **POST** /api/ai/openai/responses/input_tokens | |
|[**createResponse**](#createresponse) | **POST** /api/ai/v1/responses | |
|[**createResponseLegacy**](#createresponselegacy) | **POST** /api/ai/openai/responses | |
|[**deleteResponse**](#deleteresponse) | **DELETE** /api/ai/v1/responses/{id} | |
|[**deleteResponseLegacy**](#deleteresponselegacy) | **DELETE** /api/ai/openai/responses/{id} | |
|[**listResponseInputItems**](#listresponseinputitems) | **GET** /api/ai/v1/responses/{id}/input_items | |
|[**listResponseInputItemsLegacy**](#listresponseinputitemslegacy) | **GET** /api/ai/openai/responses/{id}/input_items | |
|[**retrieveResponse**](#retrieveresponse) | **GET** /api/ai/v1/responses/{id} | |
|[**retrieveResponseLegacy**](#retrieveresponselegacy) | **GET** /api/ai/openai/responses/{id} | |

# **cancelResponse**
> FelorxResponse cancelResponse()

Shared native Responses gateway operation.

### Example

```typescript
import {
    ResponsesApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new ResponsesApi(configuration);

let id: string; // (default to undefined)
let xFelorxAiProvider: string; //Optional server-configured provider ID or name. Stored responses remain bound to their original provider. (optional) (default to undefined)

const { status, data } = await apiInstance.cancelResponse(
    id,
    xFelorxAiProvider
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **xFelorxAiProvider** | [**string**] | Optional server-configured provider ID or name. Stored responses remain bound to their original provider. | (optional) defaults to undefined|


### Return type

**FelorxResponse**

### Authorization

[FelorxBearer](../README.md#FelorxBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |
|**400** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**404** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**413** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**429** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**500** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**502** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**503** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**504** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**401** | Authentication required; response follows the configured authentication handler. |  -  |
|**403** | Access denied. |  -  |
|**415** | Content-Type must be application/json. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cancelResponseLegacy**
> FelorxResponse cancelResponseLegacy()

Compatibility alias of the /api/ai/v1/responses operation.

### Example

```typescript
import {
    ResponsesApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new ResponsesApi(configuration);

let id: string; // (default to undefined)
let xFelorxAiProvider: string; //Optional server-configured provider ID or name. Stored responses remain bound to their original provider. (optional) (default to undefined)

const { status, data } = await apiInstance.cancelResponseLegacy(
    id,
    xFelorxAiProvider
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **xFelorxAiProvider** | [**string**] | Optional server-configured provider ID or name. Stored responses remain bound to their original provider. | (optional) defaults to undefined|


### Return type

**FelorxResponse**

### Authorization

[FelorxBearer](../README.md#FelorxBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |
|**400** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**404** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**413** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**429** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**500** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**502** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**503** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**504** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**401** | Authentication required; response follows the configured authentication handler. |  -  |
|**403** | Access denied. |  -  |
|**415** | Content-Type must be application/json. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **compactResponse**
> FelorxCompactedResponse compactResponse(felorxResponsesCompactRequest)

Shared native Responses gateway operation.

### Example

```typescript
import {
    ResponsesApi,
    Configuration,
    FelorxResponsesCompactRequest
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new ResponsesApi(configuration);

let felorxResponsesCompactRequest: FelorxResponsesCompactRequest; //JSON object, at most 8 MiB. Duplicate property names are rejected.
let xFelorxAiProvider: string; //Optional server-configured provider ID or name. Stored responses remain bound to their original provider. (optional) (default to undefined)

const { status, data } = await apiInstance.compactResponse(
    felorxResponsesCompactRequest,
    xFelorxAiProvider
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **felorxResponsesCompactRequest** | **FelorxResponsesCompactRequest**| JSON object, at most 8 MiB. Duplicate property names are rejected. | |
| **xFelorxAiProvider** | [**string**] | Optional server-configured provider ID or name. Stored responses remain bound to their original provider. | (optional) defaults to undefined|


### Return type

**FelorxCompactedResponse**

### Authorization

[FelorxBearer](../README.md#FelorxBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |
|**400** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**404** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**413** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**429** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**500** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**502** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**503** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**504** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**401** | Authentication required; response follows the configured authentication handler. |  -  |
|**403** | Access denied. |  -  |
|**415** | Content-Type must be application/json. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **compactResponseLegacy**
> FelorxCompactedResponse compactResponseLegacy(felorxResponsesCompactRequest)

Compatibility alias of the /api/ai/v1/responses operation.

### Example

```typescript
import {
    ResponsesApi,
    Configuration,
    FelorxResponsesCompactRequest
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new ResponsesApi(configuration);

let felorxResponsesCompactRequest: FelorxResponsesCompactRequest; //JSON object, at most 8 MiB. Duplicate property names are rejected.
let xFelorxAiProvider: string; //Optional server-configured provider ID or name. Stored responses remain bound to their original provider. (optional) (default to undefined)

const { status, data } = await apiInstance.compactResponseLegacy(
    felorxResponsesCompactRequest,
    xFelorxAiProvider
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **felorxResponsesCompactRequest** | **FelorxResponsesCompactRequest**| JSON object, at most 8 MiB. Duplicate property names are rejected. | |
| **xFelorxAiProvider** | [**string**] | Optional server-configured provider ID or name. Stored responses remain bound to their original provider. | (optional) defaults to undefined|


### Return type

**FelorxCompactedResponse**

### Authorization

[FelorxBearer](../README.md#FelorxBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |
|**400** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**404** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**413** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**429** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**500** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**502** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**503** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**504** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**401** | Authentication required; response follows the configured authentication handler. |  -  |
|**403** | Access denied. |  -  |
|**415** | Content-Type must be application/json. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **countResponseInputTokens**
> FelorxResponseInputTokens countResponseInputTokens(felorxResponsesCountRequest)

Shared native Responses gateway operation.

### Example

```typescript
import {
    ResponsesApi,
    Configuration,
    FelorxResponsesCountRequest
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new ResponsesApi(configuration);

let felorxResponsesCountRequest: FelorxResponsesCountRequest; //JSON object, at most 8 MiB. Duplicate property names are rejected.
let xFelorxAiProvider: string; //Optional server-configured provider ID or name. Stored responses remain bound to their original provider. (optional) (default to undefined)

const { status, data } = await apiInstance.countResponseInputTokens(
    felorxResponsesCountRequest,
    xFelorxAiProvider
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **felorxResponsesCountRequest** | **FelorxResponsesCountRequest**| JSON object, at most 8 MiB. Duplicate property names are rejected. | |
| **xFelorxAiProvider** | [**string**] | Optional server-configured provider ID or name. Stored responses remain bound to their original provider. | (optional) defaults to undefined|


### Return type

**FelorxResponseInputTokens**

### Authorization

[FelorxBearer](../README.md#FelorxBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |
|**400** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**404** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**413** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**429** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**500** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**502** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**503** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**504** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**401** | Authentication required; response follows the configured authentication handler. |  -  |
|**403** | Access denied. |  -  |
|**415** | Content-Type must be application/json. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **countResponseInputTokensLegacy**
> FelorxResponseInputTokens countResponseInputTokensLegacy(felorxResponsesCountRequest)

Compatibility alias of the /api/ai/v1/responses operation.

### Example

```typescript
import {
    ResponsesApi,
    Configuration,
    FelorxResponsesCountRequest
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new ResponsesApi(configuration);

let felorxResponsesCountRequest: FelorxResponsesCountRequest; //JSON object, at most 8 MiB. Duplicate property names are rejected.
let xFelorxAiProvider: string; //Optional server-configured provider ID or name. Stored responses remain bound to their original provider. (optional) (default to undefined)

const { status, data } = await apiInstance.countResponseInputTokensLegacy(
    felorxResponsesCountRequest,
    xFelorxAiProvider
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **felorxResponsesCountRequest** | **FelorxResponsesCountRequest**| JSON object, at most 8 MiB. Duplicate property names are rejected. | |
| **xFelorxAiProvider** | [**string**] | Optional server-configured provider ID or name. Stored responses remain bound to their original provider. | (optional) defaults to undefined|


### Return type

**FelorxResponseInputTokens**

### Authorization

[FelorxBearer](../README.md#FelorxBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |
|**400** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**404** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**413** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**429** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**500** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**502** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**503** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**504** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**401** | Authentication required; response follows the configured authentication handler. |  -  |
|**403** | Access denied. |  -  |
|**415** | Content-Type must be application/json. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createResponse**
> FelorxResponse createResponse(felorxResponsesCreateRequest)

Shared native Responses gateway operation.

### Example

```typescript
import {
    ResponsesApi,
    Configuration,
    FelorxResponsesCreateRequest
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new ResponsesApi(configuration);

let felorxResponsesCreateRequest: FelorxResponsesCreateRequest; //JSON object, at most 8 MiB. Duplicate property names are rejected.
let xFelorxAiProvider: string; //Optional server-configured provider ID or name. Stored responses remain bound to their original provider. (optional) (default to undefined)

const { status, data } = await apiInstance.createResponse(
    felorxResponsesCreateRequest,
    xFelorxAiProvider
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **felorxResponsesCreateRequest** | **FelorxResponsesCreateRequest**| JSON object, at most 8 MiB. Duplicate property names are rejected. | |
| **xFelorxAiProvider** | [**string**] | Optional server-configured provider ID or name. Stored responses remain bound to their original provider. | (optional) defaults to undefined|


### Return type

**FelorxResponse**

### Authorization

[FelorxBearer](../README.md#FelorxBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/event-stream


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |
|**400** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**404** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**413** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**429** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**500** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**502** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**503** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**504** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**401** | Authentication required; response follows the configured authentication handler. |  -  |
|**403** | Access denied. |  -  |
|**415** | Content-Type must be application/json. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **createResponseLegacy**
> FelorxResponse createResponseLegacy(felorxResponsesCreateRequest)

Compatibility alias of the /api/ai/v1/responses operation.

### Example

```typescript
import {
    ResponsesApi,
    Configuration,
    FelorxResponsesCreateRequest
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new ResponsesApi(configuration);

let felorxResponsesCreateRequest: FelorxResponsesCreateRequest; //JSON object, at most 8 MiB. Duplicate property names are rejected.
let xFelorxAiProvider: string; //Optional server-configured provider ID or name. Stored responses remain bound to their original provider. (optional) (default to undefined)

const { status, data } = await apiInstance.createResponseLegacy(
    felorxResponsesCreateRequest,
    xFelorxAiProvider
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **felorxResponsesCreateRequest** | **FelorxResponsesCreateRequest**| JSON object, at most 8 MiB. Duplicate property names are rejected. | |
| **xFelorxAiProvider** | [**string**] | Optional server-configured provider ID or name. Stored responses remain bound to their original provider. | (optional) defaults to undefined|


### Return type

**FelorxResponse**

### Authorization

[FelorxBearer](../README.md#FelorxBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/event-stream


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |
|**400** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**404** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**413** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**429** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**500** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**502** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**503** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**504** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**401** | Authentication required; response follows the configured authentication handler. |  -  |
|**403** | Access denied. |  -  |
|**415** | Content-Type must be application/json. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteResponse**
> FelorxDeletedResponse deleteResponse()

Shared native Responses gateway operation.

### Example

```typescript
import {
    ResponsesApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new ResponsesApi(configuration);

let id: string; // (default to undefined)
let xFelorxAiProvider: string; //Optional server-configured provider ID or name. Stored responses remain bound to their original provider. (optional) (default to undefined)

const { status, data } = await apiInstance.deleteResponse(
    id,
    xFelorxAiProvider
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **xFelorxAiProvider** | [**string**] | Optional server-configured provider ID or name. Stored responses remain bound to their original provider. | (optional) defaults to undefined|


### Return type

**FelorxDeletedResponse**

### Authorization

[FelorxBearer](../README.md#FelorxBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |
|**400** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**404** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**413** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**429** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**500** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**502** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**503** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**504** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**401** | Authentication required; response follows the configured authentication handler. |  -  |
|**403** | Access denied. |  -  |
|**415** | Content-Type must be application/json. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteResponseLegacy**
> FelorxDeletedResponse deleteResponseLegacy()

Compatibility alias of the /api/ai/v1/responses operation.

### Example

```typescript
import {
    ResponsesApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new ResponsesApi(configuration);

let id: string; // (default to undefined)
let xFelorxAiProvider: string; //Optional server-configured provider ID or name. Stored responses remain bound to their original provider. (optional) (default to undefined)

const { status, data } = await apiInstance.deleteResponseLegacy(
    id,
    xFelorxAiProvider
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **xFelorxAiProvider** | [**string**] | Optional server-configured provider ID or name. Stored responses remain bound to their original provider. | (optional) defaults to undefined|


### Return type

**FelorxDeletedResponse**

### Authorization

[FelorxBearer](../README.md#FelorxBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |
|**400** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**404** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**413** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**429** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**500** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**502** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**503** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**504** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**401** | Authentication required; response follows the configured authentication handler. |  -  |
|**403** | Access denied. |  -  |
|**415** | Content-Type must be application/json. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **listResponseInputItems**
> FelorxResponseInputItems listResponseInputItems()

Shared native Responses gateway operation.

### Example

```typescript
import {
    ResponsesApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new ResponsesApi(configuration);

let id: string; // (default to undefined)
let after: string; // (optional) (default to undefined)
let limit: number; // (optional) (default to undefined)
let order: string; // (optional) (default to undefined)
let xFelorxAiProvider: string; //Optional server-configured provider ID or name. Stored responses remain bound to their original provider. (optional) (default to undefined)

const { status, data } = await apiInstance.listResponseInputItems(
    id,
    after,
    limit,
    order,
    xFelorxAiProvider
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **after** | [**string**] |  | (optional) defaults to undefined|
| **limit** | [**number**] |  | (optional) defaults to undefined|
| **order** | [**string**] |  | (optional) defaults to undefined|
| **xFelorxAiProvider** | [**string**] | Optional server-configured provider ID or name. Stored responses remain bound to their original provider. | (optional) defaults to undefined|


### Return type

**FelorxResponseInputItems**

### Authorization

[FelorxBearer](../README.md#FelorxBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |
|**400** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**404** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**413** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**429** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**500** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**502** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**503** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**504** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**401** | Authentication required; response follows the configured authentication handler. |  -  |
|**403** | Access denied. |  -  |
|**415** | Content-Type must be application/json. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **listResponseInputItemsLegacy**
> FelorxResponseInputItems listResponseInputItemsLegacy()

Compatibility alias of the /api/ai/v1/responses operation.

### Example

```typescript
import {
    ResponsesApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new ResponsesApi(configuration);

let id: string; // (default to undefined)
let after: string; // (optional) (default to undefined)
let limit: number; // (optional) (default to undefined)
let order: string; // (optional) (default to undefined)
let xFelorxAiProvider: string; //Optional server-configured provider ID or name. Stored responses remain bound to their original provider. (optional) (default to undefined)

const { status, data } = await apiInstance.listResponseInputItemsLegacy(
    id,
    after,
    limit,
    order,
    xFelorxAiProvider
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **after** | [**string**] |  | (optional) defaults to undefined|
| **limit** | [**number**] |  | (optional) defaults to undefined|
| **order** | [**string**] |  | (optional) defaults to undefined|
| **xFelorxAiProvider** | [**string**] | Optional server-configured provider ID or name. Stored responses remain bound to their original provider. | (optional) defaults to undefined|


### Return type

**FelorxResponseInputItems**

### Authorization

[FelorxBearer](../README.md#FelorxBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |
|**400** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**404** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**413** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**429** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**500** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**502** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**503** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**504** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**401** | Authentication required; response follows the configured authentication handler. |  -  |
|**403** | Access denied. |  -  |
|**415** | Content-Type must be application/json. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **retrieveResponse**
> FelorxResponse retrieveResponse()

Shared native Responses gateway operation.

### Example

```typescript
import {
    ResponsesApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new ResponsesApi(configuration);

let id: string; // (default to undefined)
let xFelorxAiProvider: string; //Optional server-configured provider ID or name. Stored responses remain bound to their original provider. (optional) (default to undefined)

const { status, data } = await apiInstance.retrieveResponse(
    id,
    xFelorxAiProvider
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **xFelorxAiProvider** | [**string**] | Optional server-configured provider ID or name. Stored responses remain bound to their original provider. | (optional) defaults to undefined|


### Return type

**FelorxResponse**

### Authorization

[FelorxBearer](../README.md#FelorxBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |
|**400** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**404** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**413** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**429** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**500** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**502** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**503** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**504** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**401** | Authentication required; response follows the configured authentication handler. |  -  |
|**403** | Access denied. |  -  |
|**415** | Content-Type must be application/json. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **retrieveResponseLegacy**
> FelorxResponse retrieveResponseLegacy()

Compatibility alias of the /api/ai/v1/responses operation.

### Example

```typescript
import {
    ResponsesApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new ResponsesApi(configuration);

let id: string; // (default to undefined)
let xFelorxAiProvider: string; //Optional server-configured provider ID or name. Stored responses remain bound to their original provider. (optional) (default to undefined)

const { status, data } = await apiInstance.retrieveResponseLegacy(
    id,
    xFelorxAiProvider
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|
| **xFelorxAiProvider** | [**string**] | Optional server-configured provider ID or name. Stored responses remain bound to their original provider. | (optional) defaults to undefined|


### Return type

**FelorxResponse**

### Authorization

[FelorxBearer](../README.md#FelorxBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful response |  -  |
|**400** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**404** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**413** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**429** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**500** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**502** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**503** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**504** | Request or service failure. Validation middleware may use the host validation error format. |  -  |
|**401** | Authentication required; response follows the configured authentication handler. |  -  |
|**403** | Access denied. |  -  |
|**415** | Content-Type must be application/json. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

