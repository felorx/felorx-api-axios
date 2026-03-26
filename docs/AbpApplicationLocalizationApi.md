# AbpApplicationLocalizationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getAbpApplicationLocalization**](#getabpapplicationlocalization) | **GET** /api/abp/application-localization | |

# **getAbpApplicationLocalization**
> ApplicationLocalizationDto getAbpApplicationLocalization()


### Example

```typescript
import {
    AbpApplicationLocalizationApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AbpApplicationLocalizationApi(configuration);

let cultureName: string; // (default to undefined)
let onlyDynamics: boolean; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAbpApplicationLocalization(
    cultureName,
    onlyDynamics
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **cultureName** | [**string**] |  | defaults to undefined|
| **onlyDynamics** | [**boolean**] |  | (optional) defaults to undefined|


### Return type

**ApplicationLocalizationDto**

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

