# AiProviderApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createAiProvider**](#createaiprovider) | **POST** /api/app/ai-provider | |
|[**deleteAiProviderById**](#deleteaiproviderbyid) | **DELETE** /api/app/ai-provider/{id} | |
|[**getAiProviderById**](#getaiproviderbyid) | **GET** /api/app/ai-provider/{id} | |
|[**getAiProviderList**](#getaiproviderlist) | **GET** /api/app/ai-provider | |
|[**setDefaultModelPostApiAppAiProviderSetDefaultModel**](#setdefaultmodelpostapiappaiprovidersetdefaultmodel) | **POST** /api/app/ai-provider/set-default-model | |
|[**setEnabledPostApiAppAiProviderIdSetEnabled**](#setenabledpostapiappaiprovideridsetenabled) | **POST** /api/app/ai-provider/{id}/set-enabled | |
|[**testPostApiAppAiProviderIdTest**](#testpostapiappaiprovideridtest) | **POST** /api/app/ai-provider/{id}/test | |
|[**updateAiProvider**](#updateaiprovider) | **PUT** /api/app/ai-provider/{id} | |

# **createAiProvider**
> AiProviderDto createAiProvider()


### Example

```typescript
import {
    AiProviderApi,
    Configuration,
    CreateOrUpdateAiProviderDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AiProviderApi(configuration);

let createOrUpdateAiProviderDto: CreateOrUpdateAiProviderDto; // (optional)

const { status, data } = await apiInstance.createAiProvider(
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
|**403** | Forbidden |  -  |
|**401** | Unauthorized |  -  |
|**400** | Bad Request |  -  |
|**404** | Not Found |  -  |
|**501** | Server Error |  -  |
|**500** | Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **deleteAiProviderById**
> deleteAiProviderById()


### Example

```typescript
import {
    AiProviderApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AiProviderApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteAiProviderById(
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

# **getAiProviderById**
> AiProviderDto getAiProviderById()


### Example

```typescript
import {
    AiProviderApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AiProviderApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getAiProviderById(
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
|**403** | Forbidden |  -  |
|**401** | Unauthorized |  -  |
|**400** | Bad Request |  -  |
|**404** | Not Found |  -  |
|**501** | Server Error |  -  |
|**500** | Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getAiProviderList**
> AiProviderDtoPagedResultDto getAiProviderList()


### Example

```typescript
import {
    AiProviderApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AiProviderApi(configuration);

let filter: string; // (optional) (default to undefined)
let providerType: AiProviderType; // (optional) (default to undefined)
let capability: AiCapability; // (optional) (default to undefined)
let enabled: boolean; // (optional) (default to undefined)
let sorting: string; // (optional) (default to undefined)
let skipCount: number; // (optional) (default to undefined)
let maxResultCount: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAiProviderList(
    filter,
    providerType,
    capability,
    enabled,
    sorting,
    skipCount,
    maxResultCount
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **filter** | [**string**] |  | (optional) defaults to undefined|
| **providerType** | **AiProviderType** |  | (optional) defaults to undefined|
| **capability** | **AiCapability** |  | (optional) defaults to undefined|
| **enabled** | [**boolean**] |  | (optional) defaults to undefined|
| **sorting** | [**string**] |  | (optional) defaults to undefined|
| **skipCount** | [**number**] |  | (optional) defaults to undefined|
| **maxResultCount** | [**number**] |  | (optional) defaults to undefined|


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
|**403** | Forbidden |  -  |
|**401** | Unauthorized |  -  |
|**400** | Bad Request |  -  |
|**404** | Not Found |  -  |
|**501** | Server Error |  -  |
|**500** | Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **setDefaultModelPostApiAppAiProviderSetDefaultModel**
> AiProviderDto setDefaultModelPostApiAppAiProviderSetDefaultModel()


### Example

```typescript
import {
    AiProviderApi,
    Configuration,
    SetDefaultAiModelDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AiProviderApi(configuration);

let setDefaultAiModelDto: SetDefaultAiModelDto; // (optional)

const { status, data } = await apiInstance.setDefaultModelPostApiAppAiProviderSetDefaultModel(
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
|**403** | Forbidden |  -  |
|**401** | Unauthorized |  -  |
|**400** | Bad Request |  -  |
|**404** | Not Found |  -  |
|**501** | Server Error |  -  |
|**500** | Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **setEnabledPostApiAppAiProviderIdSetEnabled**
> AiProviderDto setEnabledPostApiAppAiProviderIdSetEnabled()


### Example

```typescript
import {
    AiProviderApi,
    Configuration,
    SetAiProviderEnabledDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AiProviderApi(configuration);

let id: string; // (default to undefined)
let setAiProviderEnabledDto: SetAiProviderEnabledDto; // (optional)

const { status, data } = await apiInstance.setEnabledPostApiAppAiProviderIdSetEnabled(
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
|**403** | Forbidden |  -  |
|**401** | Unauthorized |  -  |
|**400** | Bad Request |  -  |
|**404** | Not Found |  -  |
|**501** | Server Error |  -  |
|**500** | Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **testPostApiAppAiProviderIdTest**
> AiProviderDto testPostApiAppAiProviderIdTest()


### Example

```typescript
import {
    AiProviderApi,
    Configuration,
    TestAiProviderDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AiProviderApi(configuration);

let id: string; // (default to undefined)
let testAiProviderDto: TestAiProviderDto; // (optional)

const { status, data } = await apiInstance.testPostApiAppAiProviderIdTest(
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
|**403** | Forbidden |  -  |
|**401** | Unauthorized |  -  |
|**400** | Bad Request |  -  |
|**404** | Not Found |  -  |
|**501** | Server Error |  -  |
|**500** | Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateAiProvider**
> AiProviderDto updateAiProvider()


### Example

```typescript
import {
    AiProviderApi,
    Configuration,
    CreateOrUpdateAiProviderDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AiProviderApi(configuration);

let id: string; // (default to undefined)
let createOrUpdateAiProviderDto: CreateOrUpdateAiProviderDto; // (optional)

const { status, data } = await apiInstance.updateAiProvider(
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
|**403** | Forbidden |  -  |
|**401** | Unauthorized |  -  |
|**400** | Bad Request |  -  |
|**404** | Not Found |  -  |
|**501** | Server Error |  -  |
|**500** | Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

