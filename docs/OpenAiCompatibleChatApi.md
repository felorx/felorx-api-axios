# OpenAiCompatibleChatApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createPostApiAiV1ChatCompletions**](#createpostapiaiv1chatcompletions) | **POST** /api/ai/v1/chat/completions | |

# **createPostApiAiV1ChatCompletions**
> AiChatCompletionDto createPostApiAiV1ChatCompletions()


### Example

```typescript
import {
    OpenAiCompatibleChatApi,
    Configuration,
    OpenAiChatCompletionRequestDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new OpenAiCompatibleChatApi(configuration);

let openAiChatCompletionRequestDto: OpenAiChatCompletionRequestDto; // (optional)

const { status, data } = await apiInstance.createPostApiAiV1ChatCompletions(
    openAiChatCompletionRequestDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **openAiChatCompletionRequestDto** | **OpenAiChatCompletionRequestDto**|  | |


### Return type

**AiChatCompletionDto**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

