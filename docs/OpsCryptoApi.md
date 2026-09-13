# OpsCryptoApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getVault**](#getvault) | **GET** /api/app/ops-crypto/vault | |
|[**putVault**](#putvault) | **PUT** /api/app/ops-crypto/vault | |

# **getVault**
> OpsCryptoVaultDto getVault()


### Example

```typescript
import {
    OpsCryptoApi,
    Configuration
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new OpsCryptoApi(configuration);

const { status, data } = await apiInstance.getVault();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**OpsCryptoVaultDto**

### Authorization

No authorization required

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

# **putVault**
> putVault()


### Example

```typescript
import {
    OpsCryptoApi,
    Configuration,
    OpsCryptoVaultDto
} from 'felorx-api';

const configuration = new Configuration();
const apiInstance = new OpsCryptoApi(configuration);

let opsCryptoVaultDto: OpsCryptoVaultDto; // (optional)

const { status, data } = await apiInstance.putVault(
    opsCryptoVaultDto
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **opsCryptoVaultDto** | **OpsCryptoVaultDto**|  | |


### Return type

void (empty response body)

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

