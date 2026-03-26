# AvatarApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createAvatar**](#createavatar) | **POST** /api/app/avatar | |
|[**getCredentials**](#getcredentials) | **GET** /api/app/avatar/credentials | |

# **createAvatar**
> AvatarDto createAvatar()


### Example

```typescript
import {
    AvatarApi,
    Configuration,
    CreateAvatarDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AvatarApi(configuration);

let createAvatarDto: CreateAvatarDto; // (optional)

const { status, data } = await apiInstance.createAvatar(
    createAvatarDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createAvatarDto** | **CreateAvatarDto**|  | |


### Return type

**AvatarDto**

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

# **getCredentials**
> StorageObjectCredentials getCredentials()


### Example

```typescript
import {
    AvatarApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AvatarApi(configuration);

let key: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getCredentials(
    key
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **key** | [**string**] |  | (optional) defaults to undefined|


### Return type

**StorageObjectCredentials**

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

