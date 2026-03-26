# RemoteServiceErrorInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **string** |  | [optional] [default to undefined]
**message** | **string** |  | [optional] [default to undefined]
**details** | **string** |  | [optional] [default to undefined]
**data** | **{ [key: string]: any | undefined; }** |  | [optional] [default to undefined]
**validationErrors** | [**Array&lt;RemoteServiceValidationErrorInfo&gt;**](RemoteServiceValidationErrorInfo.md) |  | [optional] [default to undefined]

## Example

```typescript
import { RemoteServiceErrorInfo } from 'puupee-api';

const instance: RemoteServiceErrorInfo = {
    code,
    message,
    details,
    data,
    validationErrors,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
