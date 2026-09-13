# RemotePairingApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**issueAssertion**](#issueassertion) | **POST** /api/app/remote-pairing/issue-assertion | |
|[**verifyAssertion**](#verifyassertion) | **POST** /api/app/remote-pairing/verify-assertion | |

# **issueAssertion**
> RemotePairingAssertionDto issueAssertion()


### Example

```typescript
import {
    RemotePairingApi,
    Configuration,
    RemotePairingBindingDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new RemotePairingApi(configuration);

let remotePairingBindingDto: RemotePairingBindingDto; // (optional)

const { status, data } = await apiInstance.issueAssertion(
    remotePairingBindingDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **remotePairingBindingDto** | **RemotePairingBindingDto**|  | |


### Return type

**RemotePairingAssertionDto**

### Authorization

No authorization required

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

# **verifyAssertion**
> RemotePairingVerificationDto verifyAssertion()


### Example

```typescript
import {
    RemotePairingApi,
    Configuration,
    VerifyRemotePairingAssertionDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new RemotePairingApi(configuration);

let verifyRemotePairingAssertionDto: VerifyRemotePairingAssertionDto; // (optional)

const { status, data } = await apiInstance.verifyAssertion(
    verifyRemotePairingAssertionDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **verifyRemotePairingAssertionDto** | **VerifyRemotePairingAssertionDto**|  | |


### Return type

**RemotePairingVerificationDto**

### Authorization

No authorization required

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

