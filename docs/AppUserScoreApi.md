# AppUserScoreApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createAppUserScore**](#createappuserscore) | **POST** /api/app/app-user-score | |

# **createAppUserScore**
> AppUserScoreDto createAppUserScore()


### Example

```typescript
import {
    AppUserScoreApi,
    Configuration,
    CreateOrUpdateAppUserScoreDto
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AppUserScoreApi(configuration);

let createOrUpdateAppUserScoreDto: CreateOrUpdateAppUserScoreDto; // (optional)

const { status, data } = await apiInstance.createAppUserScore(
    createOrUpdateAppUserScoreDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **createOrUpdateAppUserScoreDto** | **CreateOrUpdateAppUserScoreDto**|  | |


### Return type

**AppUserScoreDto**

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

