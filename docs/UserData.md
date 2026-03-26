# UserData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional] [default to undefined]
**tenantId** | **string** |  | [optional] [default to undefined]
**userName** | **string** |  | [optional] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**surname** | **string** |  | [optional] [default to undefined]
**isActive** | **boolean** |  | [optional] [default to undefined]
**email** | **string** |  | [optional] [default to undefined]
**emailConfirmed** | **boolean** |  | [optional] [default to undefined]
**phoneNumber** | **string** |  | [optional] [default to undefined]
**phoneNumberConfirmed** | **boolean** |  | [optional] [default to undefined]
**extraProperties** | **{ [key: string]: any | undefined; }** |  | [optional] [readonly] [default to undefined]

## Example

```typescript
import { UserData } from 'puupee-api';

const instance: UserData = {
    id,
    tenantId,
    userName,
    name,
    surname,
    isActive,
    email,
    emailConfirmed,
    phoneNumber,
    phoneNumberConfirmed,
    extraProperties,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
