# UpdateEmailSettingsDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**smtpHost** | **string** |  | [optional] [default to undefined]
**smtpPort** | **number** |  | [optional] [default to undefined]
**smtpUserName** | **string** |  | [optional] [default to undefined]
**smtpPassword** | **string** |  | [optional] [default to undefined]
**smtpDomain** | **string** |  | [optional] [default to undefined]
**smtpEnableSsl** | **boolean** |  | [optional] [default to undefined]
**smtpUseDefaultCredentials** | **boolean** |  | [optional] [default to undefined]
**defaultFromAddress** | **string** |  | [default to undefined]
**defaultFromDisplayName** | **string** |  | [default to undefined]

## Example

```typescript
import { UpdateEmailSettingsDto } from 'puupee-api';

const instance: UpdateEmailSettingsDto = {
    smtpHost,
    smtpPort,
    smtpUserName,
    smtpPassword,
    smtpDomain,
    smtpEnableSsl,
    smtpUseDefaultCredentials,
    defaultFromAddress,
    defaultFromDisplayName,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
