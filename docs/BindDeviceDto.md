# BindDeviceDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**token** | **string** |  | [optional] [default to undefined]
**isPhysicalDevice** | **boolean** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**platform** | [**AppPlatform**](AppPlatform.md) |  | [optional] [default to undefined]
**brand** | **string** |  | [optional] [default to undefined]
**systemVersion** | **string** |  | [optional] [default to undefined]
**appName** | **string** | 发起绑定的应用名。服务端优先使用访问令牌中的可信 app_name 声明。 | [optional] [default to undefined]

## Example

```typescript
import { BindDeviceDto } from 'felorx-api';

const instance: BindDeviceDto = {
    token,
    isPhysicalDevice,
    name,
    platform,
    brand,
    systemVersion,
    appName,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
