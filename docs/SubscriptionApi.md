# SubscriptionApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**alipayNotify**](#alipaynotify) | **POST** /api/app/alipay/notify | 支付宝异步通知。成功时必须返回纯文本 success，否则支付宝会重试通知。|
|[**appleNotifications**](#applenotifications) | **POST** /api/app/subscription/apple-notifications | 苹果订阅 Callback 地址|
|[**capturePayPalOrder**](#capturepaypalorder) | **POST** /api/app/subscription/capture-pay-pal-order | 捕获 PayPal 订单并完成订阅|
|[**createAlipayOrderPostApiAppSubscriptionAlipayOrder**](#createalipayorderpostapiappsubscriptionalipayorder) | **POST** /api/app/subscription/alipay-order | 创建支付宝一次性支付订单|
|[**createOrder**](#createorder) | **POST** /api/app/subscription/order | |
|[**createPayPalOrderPostApiAppSubscriptionPayPalOrder**](#createpaypalorderpostapiappsubscriptionpaypalorder) | **POST** /api/app/subscription/pay-pal-order | 创建 PayPal 订单|
|[**getPlanPrices**](#getplanprices) | **GET** /api/app/subscription/plan-prices/by-app-id/{appId} | 获取应用对客户端开放的订阅售卖价格。|
|[**getStoreProducts**](#getstoreproducts) | **GET** /api/app/subscription/store-products/by-app-id/{appId} | 获取客户端商店购买所需的启用商品映射。商品 ID 本身属于公开商店元数据。|
|[**getSubscriptionById**](#getsubscriptionbyid) | **GET** /api/app/subscription | |
|[**getSubscriptionList**](#getsubscriptionlist) | **GET** /api/app/subscription/list | 获取用户订阅列表，每个应用只返回最新的一条订阅记录（含有效和已过期的）|
|[**payPalReturn**](#paypalreturn) | **GET** /api/app/paypal/notify | PayPal 浏览器审批后的返回入口。用于桌面/移动 App 跳转外部浏览器时免网站登录完成确认。|
|[**payPalWebhook**](#paypalwebhook) | **POST** /api/app/paypal/notify | PayPal webhook. Configure PayPal:WebhookId to enable signature verification.|
|[**verifyReceipt**](#verifyreceipt) | **POST** /api/app/subscription/verify-receipt | |

# **alipayNotify**
> string alipayNotify()


### Example

```typescript
import {
    SubscriptionApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionApi(configuration);

const { status, data } = await apiInstance.alipayNotify();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**string**

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

# **appleNotifications**
> appleNotifications()


### Example

```typescript
import {
    SubscriptionApi,
    Configuration,
    AppleNotificaionDto
} from 'felorx-api';

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

# **capturePayPalOrder**
> SubscriptionDto capturePayPalOrder()


### Example

```typescript
import {
    SubscriptionApi,
    Configuration,
    CapturePayPalOrderDto
} from 'felorx-api';

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

# **createAlipayOrderPostApiAppSubscriptionAlipayOrder**
> CreateAlipayOrderResultDto createAlipayOrderPostApiAppSubscriptionAlipayOrder()


### Example

```typescript
import {
    SubscriptionApi,
    Configuration,
    CreateAlipayOrderDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionApi(configuration);

let createAlipayOrderDto: CreateAlipayOrderDto; // (optional)

const { status, data } = await apiInstance.createAlipayOrderPostApiAppSubscriptionAlipayOrder(
    createAlipayOrderDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createAlipayOrderDto** | **CreateAlipayOrderDto**|  | |


### Return type

**CreateAlipayOrderResultDto**

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

# **createOrder**
> SubscriptionOrderDto createOrder()


### Example

```typescript
import {
    SubscriptionApi,
    Configuration,
    CreateOrGetSubscriptionOrderDto
} from 'felorx-api';

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

# **createPayPalOrderPostApiAppSubscriptionPayPalOrder**
> CreatePayPalOrderResultDto createPayPalOrderPostApiAppSubscriptionPayPalOrder()


### Example

```typescript
import {
    SubscriptionApi,
    Configuration,
    CreatePayPalOrderDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionApi(configuration);

let createPayPalOrderDto: CreatePayPalOrderDto; // (optional)

const { status, data } = await apiInstance.createPayPalOrderPostApiAppSubscriptionPayPalOrder(
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

# **getPlanPrices**
> Array<AppPlanPriceDto> getPlanPrices()


### Example

```typescript
import {
    SubscriptionApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionApi(configuration);

let appId: string; // (default to undefined)

const { status, data } = await apiInstance.getPlanPrices(
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

# **getStoreProducts**
> Array<StoreProductMappingDto> getStoreProducts()


### Example

```typescript
import {
    SubscriptionApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionApi(configuration);

let appId: string; // (default to undefined)
let provider: BillingProvider; // (optional) (default to undefined)
let platform: AppPlatform; // (optional) (default to undefined)
let environment: string; // (optional) (default to 'production')

const { status, data } = await apiInstance.getStoreProducts(
    appId,
    provider,
    platform,
    environment
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **appId** | [**string**] |  | defaults to undefined|
| **provider** | **BillingProvider** |  | (optional) defaults to undefined|
| **platform** | **AppPlatform** |  | (optional) defaults to undefined|
| **environment** | [**string**] |  | (optional) defaults to 'production'|


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

# **getSubscriptionById**
> SubscriptionDto getSubscriptionById()


### Example

```typescript
import {
    SubscriptionApi,
    Configuration
} from 'felorx-api';

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

# **getSubscriptionList**
> Array<SubscriptionDto> getSubscriptionList()


### Example

```typescript
import {
    SubscriptionApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionApi(configuration);

const { status, data } = await apiInstance.getSubscriptionList();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<SubscriptionDto>**

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

# **payPalReturn**
> payPalReturn()


### Example

```typescript
import {
    SubscriptionApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionApi(configuration);

let token: string; // (optional) (default to undefined)
let subscriptionId: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.payPalReturn(
    token,
    subscriptionId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **token** | [**string**] |  | (optional) defaults to undefined|
| **subscriptionId** | [**string**] |  | (optional) defaults to undefined|


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
|**403** | Forbidden |  -  |
|**401** | Unauthorized |  -  |
|**400** | Bad Request |  -  |
|**404** | Not Found |  -  |
|**501** | Server Error |  -  |
|**500** | Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **payPalWebhook**
> PayPalWebhookProcessResultDto payPalWebhook()


### Example

```typescript
import {
    SubscriptionApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new SubscriptionApi(configuration);

const { status, data } = await apiInstance.payPalWebhook();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**PayPalWebhookProcessResultDto**

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

# **verifyReceipt**
> VerifyReceiptResult verifyReceipt()


### Example

```typescript
import {
    SubscriptionApi,
    Configuration,
    VerifyReceiptDto
} from 'felorx-api';

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

