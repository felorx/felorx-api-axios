# AbpApplicationConfigurationApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getAbpApplicationConfiguration**](#getabpapplicationconfiguration) | **GET** /api/abp/application-configuration | |

# **getAbpApplicationConfiguration**
> ApplicationConfigurationDto getAbpApplicationConfiguration()


### Example

```typescript
import {
    AbpApplicationConfigurationApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AbpApplicationConfigurationApi(configuration);

let includeLocalizationResources: boolean; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAbpApplicationConfiguration(
    includeLocalizationResources
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **includeLocalizationResources** | [**boolean**] |  | (optional) defaults to undefined|


### Return type

**ApplicationConfigurationDto**

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

