# PermissionGrantInfoDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** |  | [optional] [default to undefined]
**displayName** | **string** |  | [optional] [default to undefined]
**parentName** | **string** |  | [optional] [default to undefined]
**isGranted** | **boolean** |  | [optional] [default to undefined]
**allowedProviders** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**grantedProviders** | [**Array&lt;ProviderInfoDto&gt;**](ProviderInfoDto.md) |  | [optional] [default to undefined]

## Example

```typescript
import { PermissionGrantInfoDto } from 'puupee-api';

const instance: PermissionGrantInfoDto = {
    name,
    displayName,
    parentName,
    isGranted,
    allowedProviders,
    grantedProviders,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
