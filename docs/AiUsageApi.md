# AiUsageApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getRecords**](#getrecords) | **GET** /api/ai/usage/records | |
|[**getSummaryGetApiAiUsageSummary**](#getsummarygetapiaiusagesummary) | **GET** /api/ai/usage/summary | |

# **getRecords**
> AiUsageRecordDtoPagedResultDto getRecords()


### Example

```typescript
import {
    AiUsageApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AiUsageApi(configuration);

let from: string; // (optional) (default to undefined)
let to: string; // (optional) (default to undefined)
let skipCount: number; // (optional) (default to 0)
let maxResultCount: number; // (optional) (default to 20)

const { status, data } = await apiInstance.getRecords(
    from,
    to,
    skipCount,
    maxResultCount
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **from** | [**string**] |  | (optional) defaults to undefined|
| **to** | [**string**] |  | (optional) defaults to undefined|
| **skipCount** | [**number**] |  | (optional) defaults to 0|
| **maxResultCount** | [**number**] |  | (optional) defaults to 20|


### Return type

**AiUsageRecordDtoPagedResultDto**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getSummaryGetApiAiUsageSummary**
> AiUsageSummaryDto getSummaryGetApiAiUsageSummary()


### Example

```typescript
import {
    AiUsageApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new AiUsageApi(configuration);

let from: string; // (optional) (default to undefined)
let to: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.getSummaryGetApiAiUsageSummary(
    from,
    to
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **from** | [**string**] |  | (optional) defaults to undefined|
| **to** | [**string**] |  | (optional) defaults to undefined|


### Return type

**AiUsageSummaryDto**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

