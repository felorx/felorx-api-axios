# SubscriptionBillingAdminApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createPlanPrice**](#createplanprice) | **POST** /api/app/subscription-billing-admin/plan-prices | |
|[**deletePlanPrice**](#deleteplanprice) | **DELETE** /api/app/subscription-billing-admin/plan-prices/{id} | |
|[**deleteStoreMapping**](#deletestoremapping) | **DELETE** /api/app/subscription-billing-admin/store-mappings/{id} | |
|[**getPlanPrice**](#getplanprice) | **GET** /api/app/subscription-billing-admin/plan-prices/{id} | |
|[**getPlanPricesByAppId**](#getplanpricesbyappid) | **GET** /api/app/subscription-billing-admin/plan-prices/by-app-id/{appId} | |
|[**getPlanPricesByPricingId**](#getplanpricesbypricingid) | **GET** /api/app/subscription-billing-admin/plan-prices/by-pricing-id/{pricingId} | |
|[**getStoreMappingsByAppId**](#getstoremappingsbyappid) | **GET** /api/app/subscription-billing-admin/store-mappings/by-app-id/{appId} | |
|[**getStoreMappingsByPlanPriceId**](#getstoremappingsbyplanpriceid) | **GET** /api/app/subscription-billing-admin/store-mappings/by-plan-price-id/{planPriceId} | |
|[**updatePlanPrice**](#updateplanprice) | **PUT** /api/app/subscription-billing-admin/plan-prices/{id} | |
|[**upsertStoreMapping**](#upsertstoremapping) | **POST** /api/app/subscription-billing-admin/store-mappings/upsert | |

# **createPlanPrice**
> AppPlanPriceDto createPlanPrice()


### Example

```typescript
import {
    SubscriptionBillingAdminApi,
    Configuration,
    CreateOrUpdateAppPlanPriceDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionBillingAdminApi(configuration);

let createOrUpdateAppPlanPriceDto: CreateOrUpdateAppPlanPriceDto; // (optional)

const { status, data } = await apiInstance.createPlanPrice(
    createOrUpdateAppPlanPriceDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateAppPlanPriceDto** | **CreateOrUpdateAppPlanPriceDto**|  | |


### Return type

**AppPlanPriceDto**

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

# **deletePlanPrice**
> deletePlanPrice()


### Example

```typescript
import {
    SubscriptionBillingAdminApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionBillingAdminApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deletePlanPrice(
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

# **deleteStoreMapping**
> deleteStoreMapping()


### Example

```typescript
import {
    SubscriptionBillingAdminApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionBillingAdminApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.deleteStoreMapping(
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

# **getPlanPrice**
> AppPlanPriceDto getPlanPrice()


### Example

```typescript
import {
    SubscriptionBillingAdminApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionBillingAdminApi(configuration);

let id: string; // (default to undefined)

const { status, data } = await apiInstance.getPlanPrice(
    id
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AppPlanPriceDto**

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

# **getPlanPricesByAppId**
> Array<AppPlanPriceDto> getPlanPricesByAppId()


### Example

```typescript
import {
    SubscriptionBillingAdminApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionBillingAdminApi(configuration);

let appId: string; // (default to undefined)

const { status, data } = await apiInstance.getPlanPricesByAppId(
    appId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appId** | [**string**] |  | defaults to undefined|


### Return type

**Array<AppPlanPriceDto>**

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

# **getPlanPricesByPricingId**
> Array<AppPlanPriceDto> getPlanPricesByPricingId()


### Example

```typescript
import {
    SubscriptionBillingAdminApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionBillingAdminApi(configuration);

let pricingId: string; // (default to undefined)

const { status, data } = await apiInstance.getPlanPricesByPricingId(
    pricingId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **pricingId** | [**string**] |  | defaults to undefined|


### Return type

**Array<AppPlanPriceDto>**

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

# **getStoreMappingsByAppId**
> Array<StoreProductMappingDto> getStoreMappingsByAppId()


### Example

```typescript
import {
    SubscriptionBillingAdminApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionBillingAdminApi(configuration);

let appId: string; // (default to undefined)

const { status, data } = await apiInstance.getStoreMappingsByAppId(
    appId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appId** | [**string**] |  | defaults to undefined|


### Return type

**Array<StoreProductMappingDto>**

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

# **getStoreMappingsByPlanPriceId**
> Array<StoreProductMappingDto> getStoreMappingsByPlanPriceId()


### Example

```typescript
import {
    SubscriptionBillingAdminApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionBillingAdminApi(configuration);

let planPriceId: string; // (default to undefined)

const { status, data } = await apiInstance.getStoreMappingsByPlanPriceId(
    planPriceId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **planPriceId** | [**string**] |  | defaults to undefined|


### Return type

**Array<StoreProductMappingDto>**

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

# **updatePlanPrice**
> AppPlanPriceDto updatePlanPrice()


### Example

```typescript
import {
    SubscriptionBillingAdminApi,
    Configuration,
    CreateOrUpdateAppPlanPriceDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionBillingAdminApi(configuration);

let id: string; // (default to undefined)
let createOrUpdateAppPlanPriceDto: CreateOrUpdateAppPlanPriceDto; // (optional)

const { status, data } = await apiInstance.updatePlanPrice(
    id,
    createOrUpdateAppPlanPriceDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateAppPlanPriceDto** | **CreateOrUpdateAppPlanPriceDto**|  | |
| **id** | [**string**] |  | defaults to undefined|


### Return type

**AppPlanPriceDto**

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

# **upsertStoreMapping**
> StoreProductMappingDto upsertStoreMapping()


### Example

```typescript
import {
    SubscriptionBillingAdminApi,
    Configuration,
    CreateOrUpdateStoreProductMappingDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionBillingAdminApi(configuration);

let createOrUpdateStoreProductMappingDto: CreateOrUpdateStoreProductMappingDto; // (optional)

const { status, data } = await apiInstance.upsertStoreMapping(
    createOrUpdateStoreProductMappingDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateStoreProductMappingDto** | **CreateOrUpdateStoreProductMappingDto**|  | |


### Return type

**StoreProductMappingDto**

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

