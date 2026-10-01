# UserStorageItemDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** |  | [optional] [default to undefined]
**title** | **string** |  | [optional] [default to undefined]
**key** | **string** | 云空间类型标识（image/video/document/todo/note/billing…），  与同步节点 GET /sync/storage 返回的 items[].key 保持一致。  客户端据此渲染本地化类型名称，不再依赖服务端返回的英文名称。 | [optional] [default to undefined]
**count** | **number** |  | [optional] [default to undefined]
**size** | **number** |  | [optional] [default to undefined]

## Example

```typescript
import { UserStorageItemDto } from 'felorx-api';

const instance: UserStorageItemDto = {
    name,
    title,
    key,
    count,
    size,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
