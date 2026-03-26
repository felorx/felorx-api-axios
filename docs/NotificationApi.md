# NotificationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**bark**](#bark) | **GET** /api/app/notification/bark/{apiKey}/{message} | Bark 推送，兼容 Bark 推送协议  TODO: 验证 API KEY 功能, 添加[个人访问令牌]功能|
|[**getNotificationList**](#getnotificationlist) | **GET** /api/app/notification | |
|[**push**](#push) | **POST** /api/app/notification/push | |

# **bark**
> bark()


### Example

```typescript
import {
    NotificationApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new NotificationApi(configuration);

let apiKey: string; //Bark apiKey, 需要申请，注意不要泄露，泄露后产生安全问题请及时移除或禁用 apiKey (default to undefined)
let message: string; //消息内容 (default to undefined)
let automaticallyCopy: number; //携带参数 automaticallyCopy=1， 收到推送时，推送内容会自动复制到粘贴板（如发现不能自动复制，可尝试重启一下手机） (optional) (default to 0)
let copy: string; //携带copy参数， 则上面两种复制操作，将只复制copy参数的值 (optional) (default to undefined)
let url: string; //点击推送将跳转到url的地址（发送时，URL参数需要编码） (optional) (default to undefined)
let isArchive: string; //指定是否需要保存推送信息到历史记录，1 为保存，其他值为不保存。\\n如果不指定这个参数，推送信息将按照APP内设置来决定是否保存。 (optional) (default to undefined)
let group: string; //指定推送消息分组，可在历史记录中按分组查看推送。 (optional) (default to undefined)
let icon: string; //指定推送消息图标, icon (仅 iOS15 或以上支持） (optional) (default to undefined)
let level: string; //设置时效性通知 active：不设置时的默认值，系统会立即亮屏显示通知。\\ntimeSensitive：时效性通知，可在专注状态下显示通知。\\npassive：仅将通知添加到通知列表，不会亮屏提醒 (optional) (default to undefined)

const { status, data } = await apiInstance.bark(
    apiKey,
    message,
    automaticallyCopy,
    copy,
    url,
    isArchive,
    group,
    icon,
    level
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **apiKey** | [**string**] | Bark apiKey, 需要申请，注意不要泄露，泄露后产生安全问题请及时移除或禁用 apiKey | defaults to undefined|
| **message** | [**string**] | 消息内容 | defaults to undefined|
| **automaticallyCopy** | [**number**] | 携带参数 automaticallyCopy&#x3D;1， 收到推送时，推送内容会自动复制到粘贴板（如发现不能自动复制，可尝试重启一下手机） | (optional) defaults to 0|
| **copy** | [**string**] | 携带copy参数， 则上面两种复制操作，将只复制copy参数的值 | (optional) defaults to undefined|
| **url** | [**string**] | 点击推送将跳转到url的地址（发送时，URL参数需要编码） | (optional) defaults to undefined|
| **isArchive** | [**string**] | 指定是否需要保存推送信息到历史记录，1 为保存，其他值为不保存。\\n如果不指定这个参数，推送信息将按照APP内设置来决定是否保存。 | (optional) defaults to undefined|
| **group** | [**string**] | 指定推送消息分组，可在历史记录中按分组查看推送。 | (optional) defaults to undefined|
| **icon** | [**string**] | 指定推送消息图标, icon (仅 iOS15 或以上支持） | (optional) defaults to undefined|
| **level** | [**string**] | 设置时效性通知 active：不设置时的默认值，系统会立即亮屏显示通知。\\ntimeSensitive：时效性通知，可在专注状态下显示通知。\\npassive：仅将通知添加到通知列表，不会亮屏提醒 | (optional) defaults to undefined|


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

# **getNotificationList**
> NotificationInfoDtoPagedResultDto getNotificationList()


### Example

```typescript
import {
    NotificationApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new NotificationApi(configuration);

let sorting: string; // (optional) (default to undefined)
let skipCount: number; // (optional) (default to undefined)
let maxResultCount: number; // (optional) (default to undefined)

const { status, data } = await apiInstance.getNotificationList(
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

**NotificationInfoDtoPagedResultDto**

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

# **push**
> push()


### Example

```typescript
import {
    NotificationApi,
    Configuration,
    CreatePushNotificationDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new NotificationApi(configuration);

let createPushNotificationDto: CreatePushNotificationDto; // (optional)

const { status, data } = await apiInstance.push(
    createPushNotificationDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createPushNotificationDto** | **CreatePushNotificationDto**|  | |


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

