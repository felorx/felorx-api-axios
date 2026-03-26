# MessagePublishDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**title** | **string** |  | [optional] [default to undefined]
**description** | **string** |  | [optional] [default to undefined]
**appId** | **string** |  | [optional] [default to undefined]
**template** | **string** | 模板名称, 包含版本号  puupee/wechat-app-msg?version&#x3D;1 微信应用消息模板  puupee/wechat-official-msg?version&#x3D;2 微信公众号消息模板 | [optional] [default to undefined]
**data** | **{ [key: string]: any | undefined; }** | JSON格式数据 | [optional] [default to undefined]

## Example

```typescript
import { MessagePublishDto } from 'puupee-api';

const instance: MessagePublishDto = {
    title,
    description,
    appId,
    template,
    data,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
