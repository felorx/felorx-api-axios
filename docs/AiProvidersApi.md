# AiProvidersApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createPostApiAiProviders**](#createpostapiaiproviders) | **POST** /api/ai/providers | |
|[**deleteById**](#deletebyid) | **DELETE** /api/ai/providers/{id} | |
|[**getById**](#getbyid) | **GET** /api/ai/providers/{id} | |
|[**getList**](#getlist) | **GET** /api/ai/providers | |
|[**setDefaultModelPostApiAiProvidersDefaultModel**](#setdefaultmodelpostapiaiprovidersdefaultmodel) | **POST** /api/ai/providers/default-model | |
|[**setEnabledPostApiAiProvidersIdEnabled**](#setenabledpostapiaiprovidersidenabled) | **POST** /api/ai/providers/{id}/enabled | |
|[**testPostApiAiProvidersIdTest**](#testpostapiaiprovidersidtest) | **POST** /api/ai/providers/{id}/test | |
|[**update**](#update) | **PUT** /api/ai/providers/{id} | |

# **createPostApiAiProviders**
> AiProviderDto createPostApiAiProviders()


### Example

```typescript
import {
    AiProvidersApi,
    Configuration,
    CreateOrUpdateAiProviderDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AiProvidersApi(configuration);

let createOrUpdateAiProviderDto: CreateOrUpdateAiProviderDto; // (optional)

const { status, data } = await apiInstance.createPostApiAiProviders(
    createOrUpdateAiProviderDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateAiProviderDto** | **CreateOrUpdateAiProviderDto**|  | |


### Return type

**AiProviderDto**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteById**
> deleteById()


### Example

```typescript
import {
    AiProvidersApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AiProvidersApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteById(
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

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getById**
> AiProviderDto getById()


### Example

```typescript
import {
    AiProvidersApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AiProvidersApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AiProviderDto**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getList**
> AiProviderDtoPagedResultDto getList()


### Example

```typescript
import {
    AiProvidersApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AiProvidersApi(configuration);

let filter: string; // (optional) (default to undefined)
let providerType: AiProviderType; // (optional) (default to undefined)
let providerType2: AiProviderType; // (optional) (default to undefined)
let capability: AiCapability; // (optional) (default to undefined)
let enabled: boolean; // (optional) (default to undefined)
let skipCount: number; // (optional) (default to 0)
let maxResultCount: number; // (optional) (default to 10)
let sorting: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getList(
    filter,
    providerType,
    providerType2,
    capability,
    enabled,
    skipCount,
    maxResultCount,
    sorting
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **filter** | [**string**] |  | (optional) defaults to undefined|
| **providerType** | **AiProviderType** |  | (optional) defaults to undefined|
| **providerType2** | **AiProviderType** |  | (optional) defaults to undefined|
| **capability** | **AiCapability** |  | (optional) defaults to undefined|
| **enabled** | [**boolean**] |  | (optional) defaults to undefined|
| **skipCount** | [**number**] |  | (optional) defaults to 0|
| **maxResultCount** | [**number**] |  | (optional) defaults to 10|
| **sorting** | [**string**] |  | (optional) defaults to undefined|


### Return type

**AiProviderDtoPagedResultDto**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **setDefaultModelPostApiAiProvidersDefaultModel**
> AiProviderDto setDefaultModelPostApiAiProvidersDefaultModel()


### Example

```typescript
import {
    AiProvidersApi,
    Configuration,
    SetDefaultAiModelDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AiProvidersApi(configuration);

let setDefaultAiModelDto: SetDefaultAiModelDto; // (optional)

const { status, data } = await apiInstance.setDefaultModelPostApiAiProvidersDefaultModel(
    setDefaultAiModelDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **setDefaultAiModelDto** | **SetDefaultAiModelDto**|  | |


### Return type

**AiProviderDto**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **setEnabledPostApiAiProvidersIdEnabled**
> AiProviderDto setEnabledPostApiAiProvidersIdEnabled()


### Example

```typescript
import {
    AiProvidersApi,
    Configuration,
    SetAiProviderEnabledDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AiProvidersApi(configuration);

let id: string; // (default to undefined)
let setAiProviderEnabledDto: SetAiProviderEnabledDto; // (optional)

const { status, data } = await apiInstance.setEnabledPostApiAiProvidersIdEnabled(
    id,
    setAiProviderEnabledDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **setAiProviderEnabledDto** | **SetAiProviderEnabledDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AiProviderDto**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **testPostApiAiProvidersIdTest**
> AiProviderDto testPostApiAiProvidersIdTest()


### Example

```typescript
import {
    AiProvidersApi,
    Configuration,
    TestAiProviderDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AiProvidersApi(configuration);

let id: string; // (default to undefined)
let testAiProviderDto: TestAiProviderDto; // (optional)

const { status, data } = await apiInstance.testPostApiAiProvidersIdTest(
    id,
    testAiProviderDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **testAiProviderDto** | **TestAiProviderDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AiProviderDto**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update**
> AiProviderDto update()


### Example

```typescript
import {
    AiProvidersApi,
    Configuration,
    CreateOrUpdateAiProviderDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AiProvidersApi(configuration);

let id: string; // (default to undefined)
let createOrUpdateAiProviderDto: CreateOrUpdateAiProviderDto; // (optional)

const { status, data } = await apiInstance.update(
    id,
    createOrUpdateAiProviderDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateAiProviderDto** | **CreateOrUpdateAiProviderDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AiProviderDto**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

