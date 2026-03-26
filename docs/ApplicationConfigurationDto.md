# ApplicationConfigurationDto


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**localization** | [**ApplicationLocalizationConfigurationDto**](ApplicationLocalizationConfigurationDto.md) |  | [optional] [default to undefined]
**auth** | [**ApplicationAuthConfigurationDto**](ApplicationAuthConfigurationDto.md) |  | [optional] [default to undefined]
**setting** | [**ApplicationSettingConfigurationDto**](ApplicationSettingConfigurationDto.md) |  | [optional] [default to undefined]
**currentUser** | [**CurrentUserDto**](CurrentUserDto.md) |  | [optional] [default to undefined]
**features** | [**ApplicationFeatureConfigurationDto**](ApplicationFeatureConfigurationDto.md) |  | [optional] [default to undefined]
**globalFeatures** | [**ApplicationGlobalFeatureConfigurationDto**](ApplicationGlobalFeatureConfigurationDto.md) |  | [optional] [default to undefined]
**multiTenancy** | [**MultiTenancyInfoDto**](MultiTenancyInfoDto.md) |  | [optional] [default to undefined]
**currentTenant** | [**CurrentTenantDto**](CurrentTenantDto.md) |  | [optional] [default to undefined]
**timing** | [**TimingDto**](TimingDto.md) |  | [optional] [default to undefined]
**clock** | [**ClockDto**](ClockDto.md) |  | [optional] [default to undefined]
**objectExtensions** | [**ObjectExtensionsDto**](ObjectExtensionsDto.md) |  | [optional] [default to undefined]
**extraProperties** | **{ [key: string]: any | undefined; }** |  | [optional] [default to undefined]

## Example

```typescript
import { ApplicationConfigurationDto } from 'puupee-api';

const instance: ApplicationConfigurationDto = {
    localization,
    auth,
    setting,
    currentUser,
    features,
    globalFeatures,
    multiTenancy,
    currentTenant,
    timing,
    clock,
    objectExtensions,
    extraProperties,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
