# EmailSettingsDto


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
**defaultFromAddress** | **string** |  | [optional] [default to undefined]
**defaultFromDisplayName** | **string** |  | [optional] [default to undefined]

## Example

```typescript
import { EmailSettingsDto } from 'puupee-api';

const instance: EmailSettingsDto = {
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
