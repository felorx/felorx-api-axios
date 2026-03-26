# SendVerificationCodeDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**codeSender** | **string** | 验证码发送器 暂时支持: SMS: 手机短信验证码 | [optional] [default to undefined]
**account** | **string** | 验证码接受者, 用户账户 | [optional] [default to undefined]
**purpose** | **string** | 验证码用途 | [optional] [default to undefined]

## Example

```typescript
import { SendVerificationCodeDto } from 'puupee-api';

const instance: SendVerificationCodeDto = {
    codeSender,
    account,
    purpose,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
