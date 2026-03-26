# IdentityUser


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional] [readonly] [default to undefined]
**extraProperties** | **{ [key: string]: any | undefined; }** |  | [optional] [readonly] [default to undefined]
**concurrencyStamp** | **string** |  | [optional] [default to undefined]
**creationTime** | **string** |  | [optional] [default to undefined]
**creatorId** | **string** |  | [optional] [default to undefined]
**lastModificationTime** | **string** |  | [optional] [default to undefined]
**lastModifierId** | **string** |  | [optional] [default to undefined]
**isDeleted** | **boolean** |  | [optional] [default to undefined]
**deleterId** | **string** |  | [optional] [default to undefined]
**deletionTime** | **string** |  | [optional] [default to undefined]
**tenantId** | **string** |  | [optional] [default to undefined]
**userName** | **string** |  | [optional] [default to undefined]
**normalizedUserName** | **string** |  | [optional] [readonly] [default to undefined]
**name** | **string** |  | [optional] [default to undefined]
**surname** | **string** |  | [optional] [default to undefined]
**email** | **string** |  | [optional] [default to undefined]
**normalizedEmail** | **string** |  | [optional] [readonly] [default to undefined]
**emailConfirmed** | **boolean** |  | [optional] [readonly] [default to undefined]
**passwordHash** | **string** |  | [optional] [readonly] [default to undefined]
**securityStamp** | **string** |  | [optional] [readonly] [default to undefined]
**isExternal** | **boolean** |  | [optional] [default to undefined]
**phoneNumber** | **string** |  | [optional] [readonly] [default to undefined]
**phoneNumberConfirmed** | **boolean** |  | [optional] [readonly] [default to undefined]
**isActive** | **boolean** |  | [optional] [readonly] [default to undefined]
**twoFactorEnabled** | **boolean** |  | [optional] [readonly] [default to undefined]
**lockoutEnd** | **string** |  | [optional] [readonly] [default to undefined]
**lockoutEnabled** | **boolean** |  | [optional] [readonly] [default to undefined]
**accessFailedCount** | **number** |  | [optional] [readonly] [default to undefined]
**shouldChangePasswordOnNextLogin** | **boolean** |  | [optional] [readonly] [default to undefined]
**entityVersion** | **number** |  | [optional] [readonly] [default to undefined]
**lastPasswordChangeTime** | **string** |  | [optional] [readonly] [default to undefined]
**roles** | [**Array&lt;IdentityUserRole&gt;**](IdentityUserRole.md) |  | [optional] [readonly] [default to undefined]
**claims** | [**Array&lt;IdentityUserClaim&gt;**](IdentityUserClaim.md) |  | [optional] [readonly] [default to undefined]
**logins** | [**Array&lt;IdentityUserLogin&gt;**](IdentityUserLogin.md) |  | [optional] [readonly] [default to undefined]
**tokens** | [**Array&lt;IdentityUserToken&gt;**](IdentityUserToken.md) |  | [optional] [readonly] [default to undefined]
**organizationUnits** | [**Array&lt;IdentityUserOrganizationUnit&gt;**](IdentityUserOrganizationUnit.md) |  | [optional] [readonly] [default to undefined]

## Example

```typescript
import { IdentityUser } from 'puupee-api';

const instance: IdentityUser = {
    id,
    extraProperties,
    concurrencyStamp,
    creationTime,
    creatorId,
    lastModificationTime,
    lastModifierId,
    isDeleted,
    deleterId,
    deletionTime,
    tenantId,
    userName,
    normalizedUserName,
    name,
    surname,
    email,
    normalizedEmail,
    emailConfirmed,
    passwordHash,
    securityStamp,
    isExternal,
    phoneNumber,
    phoneNumberConfirmed,
    isActive,
    twoFactorEnabled,
    lockoutEnd,
    lockoutEnabled,
    accessFailedCount,
    shouldChangePasswordOnNextLogin,
    entityVersion,
    lastPasswordChangeTime,
    roles,
    claims,
    logins,
    tokens,
    organizationUnits,
};
```

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
