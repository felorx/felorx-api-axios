# MessageSourceCategoryApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getMessageSourceCategoryList**](#getmessagesourcecategorylist) | **GET** /api/app/message-source-category | |

# **getMessageSourceCategoryList**
> Array<MessageSourceCategoryDto> getMessageSourceCategoryList()


### Example

```typescript
import {
    MessageSourceCategoryApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new MessageSourceCategoryApi(configuration);

const { status, data } = await apiInstance.getMessageSourceCategoryList();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<MessageSourceCategoryDto>**

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

