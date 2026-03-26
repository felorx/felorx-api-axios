# DynamicClaimsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**refresh**](#refresh) | **POST** /api/account/dynamic-claims/refresh | |

# **refresh**
> refresh()


### Example

```typescript
import {
    DynamicClaimsApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new DynamicClaimsApi(configuration);

const { status, data } = await apiInstance.refresh();
```

### Parameters
This endpoint does not have any parameters.


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

