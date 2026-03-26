# IdentityUserUpdateDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**extraProperties** | **{ [key: string]: any | undefined; }** |  | [optional] [readonly] [default to undefined]
**userName** | **string** |  | [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**surname** | **string** |  | [optional] [default to undefined]
**email** | **string** |  | [default to undefined]
**phoneNumber** | **string** |  | [optional] [default to undefined]
**isActive** | **boolean** |  | [optional] [default to undefined]
**lockoutEnabled** | **boolean** |  | [optional] [default to undefined]
**roleNames** | **Array&lt;string&gt;** |  | [optional] [default to undefined]
**password** | **string** |  | [optional] [default to undefined]
**concurrencyStamp** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { IdentityUserUpdateDto } from 'puupee-api';

const instance: IdentityUserUpdateDto = {
    extraProperties,
    userName,
    name,
    surname,
    email,
    phoneNumber,
    isActive,
    lockoutEnabled,
    roleNames,
    password,
    concurrencyStamp,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
