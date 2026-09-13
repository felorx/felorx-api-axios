# CreditApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createAlipayOrderPostApiAppCreditAlipayOrder**](#createalipayorderpostapiappcreditalipayorder) | **POST** /api/app/credit/alipay-order | |
|[**createPayPalOrderPostApiAppCreditPayPalOrder**](#createpaypalorderpostapiappcreditpaypalorder) | **POST** /api/app/credit/pay-pal-order | |
|[**getAccountGetApiAppCreditAccountAppId**](#getaccountgetapiappcreditaccountappid) | **GET** /api/app/credit/account/{appId} | |
|[**getPackages**](#getpackages) | **GET** /api/app/credit/packages/{appId} | |
|[**refund**](#refund) | **POST** /api/app/credit/refund | |
|[**spend**](#spend) | **POST** /api/app/credit/spend | |

# **createAlipayOrderPostApiAppCreditAlipayOrder**
> CreateCreditAlipayOrderResultDto createAlipayOrderPostApiAppCreditAlipayOrder()


### Example

```typescript
import {
    CreditApi,
    Configuration,
    CreateCreditAlipayOrderDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new CreditApi(configuration);

let createCreditAlipayOrderDto: CreateCreditAlipayOrderDto; // (optional)

const { status, data } = await apiInstance.createAlipayOrderPostApiAppCreditAlipayOrder(
    createCreditAlipayOrderDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createCreditAlipayOrderDto** | **CreateCreditAlipayOrderDto**|  | |


### Return type

**CreateCreditAlipayOrderResultDto**

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

# **createPayPalOrderPostApiAppCreditPayPalOrder**
> CreateCreditPayPalOrderResultDto createPayPalOrderPostApiAppCreditPayPalOrder()


### Example

```typescript
import {
    CreditApi,
    Configuration,
    CreateCreditPayPalOrderDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new CreditApi(configuration);

let createCreditPayPalOrderDto: CreateCreditPayPalOrderDto; // (optional)

const { status, data } = await apiInstance.createPayPalOrderPostApiAppCreditPayPalOrder(
    createCreditPayPalOrderDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createCreditPayPalOrderDto** | **CreateCreditPayPalOrderDto**|  | |


### Return type

**CreateCreditPayPalOrderResultDto**

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

# **getAccountGetApiAppCreditAccountAppId**
> CreditAccountDto getAccountGetApiAppCreditAccountAppId()


### Example

```typescript
import {
    CreditApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new CreditApi(configuration);

let appId: string; // (default to undefined)

const { status, data } = await apiInstance.getAccountGetApiAppCreditAccountAppId(
    appId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appId** | [**string**] |  | defaults to undefined|


### Return type

**CreditAccountDto**

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

# **getPackages**
> Array<CreditPackageDto> getPackages()


### Example

```typescript
import {
    CreditApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new CreditApi(configuration);

let appId: string; // (default to undefined)

const { status, data } = await apiInstance.getPackages(
    appId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appId** | [**string**] |  | defaults to undefined|


### Return type

**Array<CreditPackageDto>**

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

# **refund**
> AdjustCreditsResultDto refund()


### Example

```typescript
import {
    CreditApi,
    Configuration,
    AdjustCreditsDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new CreditApi(configuration);

let adjustCreditsDto: AdjustCreditsDto; // (optional)

const { status, data } = await apiInstance.refund(
    adjustCreditsDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **adjustCreditsDto** | **AdjustCreditsDto**|  | |


### Return type

**AdjustCreditsResultDto**

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

# **spend**
> AdjustCreditsResultDto spend()


### Example

```typescript
import {
    CreditApi,
    Configuration,
    AdjustCreditsDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new CreditApi(configuration);

let adjustCreditsDto: AdjustCreditsDto; // (optional)

const { status, data } = await apiInstance.spend(
    adjustCreditsDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **adjustCreditsDto** | **AdjustCreditsDto**|  | |


### Return type

**AdjustCreditsResultDto**

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

