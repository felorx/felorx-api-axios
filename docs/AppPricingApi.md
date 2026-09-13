# AppPricingApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createAppPricing**](#createapppricing) | **POST** /api/app/app-pricing | |
|[**deleteAppPricingById**](#deleteapppricingbyid) | **DELETE** /api/app/app-pricing/{id} | |
|[**getAppPricingById**](#getapppricingbyid) | **GET** /api/app/app-pricing/{id} | 获取单条定价方案详情，允许匿名访问（与列表/商店展示一致）|
|[**getAppPricingList**](#getapppricinglist) | **GET** /api/app/app-pricing | 分页获取定价方案列表，允许匿名访问|
|[**getListByAppIdGetApiAppAppPricingByAppIdAppId**](#getlistbyappidgetapiappapppricingbyappidappid) | **GET** /api/app/app-pricing/by-app-id/{appId} | 获取应用定价方案列表，允许匿名访问供未登录用户查看订阅计划|
|[**getPricingItemsByAppId**](#getpricingitemsbyappid) | **GET** /api/app/app-pricing/pricing-items-by-app-id/{appId} | 获取应用定价功能项定义（与客户端「功能对比」行一致），允许匿名访问供官网等场景展示|
|[**updateAppPricing**](#updateapppricing) | **PUT** /api/app/app-pricing/{id} | |

# **createAppPricing**
> AppPricingDto createAppPricing()


### Example

```typescript
import {
    AppPricingApi,
    Configuration,
    CreateOrUpdateAppPricingDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AppPricingApi(configuration);

let createOrUpdateAppPricingDto: CreateOrUpdateAppPricingDto; // (optional)

const { status, data } = await apiInstance.createAppPricing(
    createOrUpdateAppPricingDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateAppPricingDto** | **CreateOrUpdateAppPricingDto**|  | |


### Return type

**AppPricingDto**

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

# **deleteAppPricingById**
> deleteAppPricingById()


### Example

```typescript
import {
    AppPricingApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AppPricingApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteAppPricingById(
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

# **getAppPricingById**
> AppPricingDto getAppPricingById()


### Example

```typescript
import {
    AppPricingApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AppPricingApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getAppPricingById(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AppPricingDto**

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

# **getAppPricingList**
> AppPricingDtoPagedResultDto getAppPricingList()


### Example

```typescript
import {
    AppPricingApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AppPricingApi(configuration);

let sorting: string; // (optional) (default to undefined)
let skipCount: number; // (optional) (default to undefined)
let maxResultCount: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAppPricingList(
    sorting,
    skipCount,
    maxResultCount
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **sorting** | [**string**] |  | (optional) defaults to undefined|
| **skipCount** | [**number**] |  | (optional) defaults to undefined|
| **maxResultCount** | [**number**] |  | (optional) defaults to undefined|


### Return type

**AppPricingDtoPagedResultDto**

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

# **getListByAppIdGetApiAppAppPricingByAppIdAppId**
> Array<AppPricingDto> getListByAppIdGetApiAppAppPricingByAppIdAppId()


### Example

```typescript
import {
    AppPricingApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AppPricingApi(configuration);

let appId: string; // (default to undefined)

const { status, data } = await apiInstance.getListByAppIdGetApiAppAppPricingByAppIdAppId(
    appId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appId** | [**string**] |  | defaults to undefined|


### Return type

**Array<AppPricingDto>**

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

# **getPricingItemsByAppId**
> Array<AppPricingItemDto> getPricingItemsByAppId()


### Example

```typescript
import {
    AppPricingApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AppPricingApi(configuration);

let appId: string; // (default to undefined)

const { status, data } = await apiInstance.getPricingItemsByAppId(
    appId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appId** | [**string**] |  | defaults to undefined|


### Return type

**Array<AppPricingItemDto>**

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

# **updateAppPricing**
> AppPricingDto updateAppPricing()


### Example

```typescript
import {
    AppPricingApi,
    Configuration,
    CreateOrUpdateAppPricingDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AppPricingApi(configuration);

let id: string; // (default to undefined)
let createOrUpdateAppPricingDto: CreateOrUpdateAppPricingDto; // (optional)

const { status, data } = await apiInstance.updateAppPricing(
    id,
    createOrUpdateAppPricingDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateAppPricingDto** | **CreateOrUpdateAppPricingDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AppPricingDto**

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

