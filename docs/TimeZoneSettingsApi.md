# TimeZoneSettingsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**getTimeZoneSettings**](#gettimezonesettings) | **GET** /api/setting-management/timezone | |
|[**getTimezones**](#gettimezones) | **GET** /api/setting-management/timezone/timezones | |
|[**updateTimeZoneSettings**](#updatetimezonesettings) | **POST** /api/setting-management/timezone | |

# **getTimeZoneSettings**
> string getTimeZoneSettings()


### Example

```typescript
import {
    TimeZoneSettingsApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new TimeZoneSettingsApi(configuration);

const { status, data } = await apiInstance.getTimeZoneSettings();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**string**

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

# **getTimezones**
> Array<NameValue> getTimezones()


### Example

```typescript
import {
    TimeZoneSettingsApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new TimeZoneSettingsApi(configuration);

const { status, data } = await apiInstance.getTimezones();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**Array<NameValue>**

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

# **updateTimeZoneSettings**
> updateTimeZoneSettings()


### Example

```typescript
import {
    TimeZoneSettingsApi,
    Configuration
} from 'puupee-api';

const configuration = new Configuration();
const apiInstance = new TimeZoneSettingsApi(configuration);

let timezone: string; // (optional) (default to undefined)

const { status, data } = await apiInstance.updateTimeZoneSettings(
    timezone
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **timezone** | [**string**] |  | (optional) defaults to undefined|


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

