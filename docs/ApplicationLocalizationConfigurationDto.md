# ApplicationLocalizationConfigurationDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**values** | **{ [key: string]: { [key: string]: string | undefined; } | undefined; }** |  | [optional] [default to undefined]
**resources** | [**{ [key: string]: ApplicationLocalizationResourceDto | undefined; }**](ApplicationLocalizationResourceDto.md) |  | [optional] [default to undefined]
**languages** | [**Array&lt;LanguageInfo&gt;**](LanguageInfo.md) |  | [optional] [default to undefined]
**currentCulture** | [**CurrentCultureDto**](CurrentCultureDto.md) |  | [optional] [default to undefined]
**defaultResourceName** | **string** |  | [optional] [default to undefined]
**languagesMap** | **{ [key: string]: Array&lt;NameValue&gt; | undefined; }** |  | [optional] [default to undefined]
**languageFilesMap** | **{ [key: string]: Array&lt;NameValue&gt; | undefined; }** |  | [optional] [default to undefined]

## Example

```typescript
import { ApplicationLocalizationConfigurationDto } from 'puupee-api';

const instance: ApplicationLocalizationConfigurationDto = {
    values,
    resources,
    languages,
    currentCulture,
    defaultResourceName,
    languagesMap,
    languageFilesMap,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
