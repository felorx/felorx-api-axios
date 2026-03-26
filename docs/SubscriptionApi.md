# SubscriptionApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**appleNotifications**](#applenotifications) | **POST** /api/app/subscription/apple-notifications | 苹果订阅 Callback 地址|
|[**capturePayPalOrder**](#capturepaypalorder) | **POST** /api/app/subscription/capture-pay-pal-order | 捕获 PayPal 订单并完成订阅|
|[**createOrder**](#createorder) | **POST** /api/app/subscription/order | |
|[**createPayPalOrder**](#createpaypalorder) | **POST** /api/app/subscription/pay-pal-order | 创建 PayPal 订单|
|[**getSubscriptionById**](#getsubscriptionbyid) | **GET** /api/app/subscription | |
|[**getSubscriptionList**](#getsubscriptionlist) | **GET** /api/app/subscription/list | 获取用户订阅列表，每个应用只返回最新的一条订阅记录（含有效和已过期的）|
|[**verifyReceipt**](#verifyreceipt) | **POST** /api/app/subscription/verify-receipt | |

# **appleNotifications**
> appleNotifications()


### Example

```typescript
import {
    SubscriptionApi,
    Configuration,
    AppleNotificaionDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionApi(configuration);

let appleNotificaionDto: AppleNotificaionDto; // (optional)

const { status, data } = await apiInstance.appleNotifications(
    appleNotificaionDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appleNotificaionDto** | **AppleNotificaionDto**|  | |


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

# **capturePayPalOrder**
> SubscriptionDto capturePayPalOrder()


### Example

```typescript
import {
    SubscriptionApi,
    Configuration,
    CapturePayPalOrderDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionApi(configuration);

let capturePayPalOrderDto: CapturePayPalOrderDto; // (optional)

const { status, data } = await apiInstance.capturePayPalOrder(
    capturePayPalOrderDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **capturePayPalOrderDto** | **CapturePayPalOrderDto**|  | |


### Return type

**SubscriptionDto**

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

# **createOrder**
> SubscriptionOrderDto createOrder()


### Example

```typescript
import {
    SubscriptionApi,
    Configuration,
    CreateOrGetSubscriptionOrderDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionApi(configuration);

let createOrGetSubscriptionOrderDto: CreateOrGetSubscriptionOrderDto; // (optional)

const { status, data } = await apiInstance.createOrder(
    createOrGetSubscriptionOrderDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrGetSubscriptionOrderDto** | **CreateOrGetSubscriptionOrderDto**|  | |


### Return type

**SubscriptionOrderDto**

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

# **createPayPalOrder**
> CreatePayPalOrderResultDto createPayPalOrder()


### Example

```typescript
import {
    SubscriptionApi,
    Configuration,
    CreatePayPalOrderDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionApi(configuration);

let createPayPalOrderDto: CreatePayPalOrderDto; // (optional)

const { status, data } = await apiInstance.createPayPalOrder(
    createPayPalOrderDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createPayPalOrderDto** | **CreatePayPalOrderDto**|  | |


### Return type

**CreatePayPalOrderResultDto**

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

# **getSubscriptionById**
> SubscriptionDto getSubscriptionById()


### Example

```typescript
import {
    SubscriptionApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionApi(configuration);

let appId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getSubscriptionById(
    appId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appId** | [**string**] |  | (optional) defaults to undefined|


### Return type

**SubscriptionDto**

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

# **getSubscriptionList**
> Array<SubscriptionDto> getSubscriptionList()


### Example

```typescript
import {
    SubscriptionApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionApi(configuration);

const { status, data } = await apiInstance.getSubscriptionList();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<SubscriptionDto>**

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

# **verifyReceipt**
> VerifyReceiptResult verifyReceipt()


### Example

```typescript
import {
    SubscriptionApi,
    Configuration,
    VerifyReceiptDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionApi(configuration);

let verifyReceiptDto: VerifyReceiptDto; // (optional)

const { status, data } = await apiInstance.verifyReceipt(
    verifyReceiptDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **verifyReceiptDto** | **VerifyReceiptDto**|  | |


### Return type

**VerifyReceiptResult**

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

