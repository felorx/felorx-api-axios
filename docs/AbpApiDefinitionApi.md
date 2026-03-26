# AbpApiDefinitionApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getAbpApiDefinition**](#getabpapidefinition) | **GET** /api/abp/api-definition | |

# **getAbpApiDefinition**
> ApplicationApiDescriptionModel getAbpApiDefinition()


### Example

```typescript
import {
    AbpApiDefinitionApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new AbpApiDefinitionApi(configuration);

let includeTypes: boolean; // (optional) (default to undefined)

const { status, data } = await apiInstance.getAbpApiDefinition(
    includeTypes
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **includeTypes** | [**boolean**] |  | (optional) defaults to undefined|


### Return type

**ApplicationApiDescriptionModel**

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

