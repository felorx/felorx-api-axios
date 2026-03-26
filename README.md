## puupee-api@1.0.0

This generator creates TypeScript/JavaScript client that utilizes [axios](https://github.com/axios/axios). The generated Node module can be used in the following environments:

Environment
* Node.js
* Webpack
* Browserify

Language level
* ES5 - you must have a Promises/A+ library installed
* ES6

Module system
* CommonJS
* ES6 module system

It can be used in both TypeScript and JavaScript. In TypeScript, the definition will be automatically resolved via `package.json`. ([Reference](https://www.typescriptlang.org/docs/handbook/declaration-files/consumption.html))

### Building

To build and compile the typescript sources to javascript use:
```
npm install
npm run build
```

### Publishing

First build the package then run `npm publish`

### Consuming

navigate to the folder of your consuming project and run one of the following commands.

_published:_

```
npm install puupee-api@1.0.0 --save
```

_unPublished (not recommended):_

```
npm install PATH_TO_GENERATED_PACKAGE --save
```

### Documentation for API Endpoints

All URIs are relative to *http://localhost*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AbpApiDefinitionApi* | [**getAbpApiDefinition**](docs/AbpApiDefinitionApi.md#getabpapidefinition) | **GET** /api/abp/api-definition | 
*AbpApplicationConfigurationApi* | [**getAbpApplicationConfiguration**](docs/AbpApplicationConfigurationApi.md#getabpapplicationconfiguration) | **GET** /api/abp/application-configuration | 
*AbpApplicationLocalizationApi* | [**getAbpApplicationLocalization**](docs/AbpApplicationLocalizationApi.md#getabpapplicationlocalization) | **GET** /api/abp/application-localization | 
*AbpTenantApi* | [**findTenantById**](docs/AbpTenantApi.md#findtenantbyid) | **GET** /api/abp/multi-tenancy/tenants/by-id/{id} | 
*AbpTenantApi* | [**findTenantByName**](docs/AbpTenantApi.md#findtenantbyname) | **GET** /api/abp/multi-tenancy/tenants/by-name/{name} | 
*AccountApi* | [**changeAccountPassword**](docs/AccountApi.md#changeaccountpassword) | **POST** /api/app/account/change-password | 
*AccountApi* | [**checkSyncAuth**](docs/AccountApi.md#checksyncauth) | **POST** /api/app/account/check-sync-auth | 检查同步认证
*AccountApi* | [**destroyAccount**](docs/AccountApi.md#destroyaccount) | **POST** /api/app/account/destroy-account | 
*AccountApi* | [**getAccount**](docs/AccountApi.md#getaccount) | **GET** /api/app/account | 
*AccountApi* | [**register**](docs/AccountApi.md#register) | **POST** /api/account/register | 
*AccountApi* | [**resetPassword**](docs/AccountApi.md#resetpassword) | **POST** /api/account/reset-password | 
*AccountApi* | [**sendPasswordResetCode**](docs/AccountApi.md#sendpasswordresetcode) | **POST** /api/account/send-password-reset-code | 
*AccountApi* | [**verifyPasswordResetToken**](docs/AccountApi.md#verifypasswordresettoken) | **POST** /api/account/verify-password-reset-token | 
*ApiKeysApi* | [**createApiKeys**](docs/ApiKeysApi.md#createapikeys) | **POST** /api/api-keys | 
*ApiKeysApi* | [**deleteApiKeysById**](docs/ApiKeysApi.md#deleteapikeysbyid) | **DELETE** /api/api-keys/{id} | 
*ApiKeysApi* | [**getApiKeysById**](docs/ApiKeysApi.md#getapikeysbyid) | **GET** /api/api-keys/{id} | 
*ApiKeysApi* | [**getApiKeysList**](docs/ApiKeysApi.md#getapikeyslist) | **GET** /api/api-keys | 
*ApiKeysApi* | [**updateApiKeys**](docs/ApiKeysApi.md#updateapikeys) | **PUT** /api/api-keys/{id} | 
*AppApi* | [**createApp**](docs/AppApi.md#createapp) | **POST** /api/app/app | 
*AppApi* | [**deleteAppById**](docs/AppApi.md#deleteappbyid) | **DELETE** /api/app/app/{id} | 
*AppApi* | [**getAppById**](docs/AppApi.md#getappbyid) | **GET** /api/app/app/{id} | 
*AppApi* | [**getAppList**](docs/AppApi.md#getapplist) | **GET** /api/app/app | 
*AppApi* | [**getByName**](docs/AppApi.md#getbyname) | **GET** /api/app/app/by-name | 
*AppApi* | [**getFeatureList**](docs/AppApi.md#getfeaturelist) | **GET** /api/app/app/feature-list/{appId} | 
*AppApi* | [**getListByDeveloperAll**](docs/AppApi.md#getlistbydeveloperall) | **GET** /api/app/app/by-developer-all | 
*AppApi* | [**getListPublic**](docs/AppApi.md#getlistpublic) | **GET** /api/app/app/public | 
*AppApi* | [**getListWithUser**](docs/AppApi.md#getlistwithuser) | **GET** /api/app/app/with-user | 
*AppApi* | [**getSdksById**](docs/AppApi.md#getsdksbyid) | **GET** /api/app/app/sdks-by-id/{appId} | 
*AppApi* | [**getUploadCredentials**](docs/AppApi.md#getuploadcredentials) | **GET** /api/app/app/upload-credentials | 
*AppApi* | [**getWithUser**](docs/AppApi.md#getwithuser) | **GET** /api/app/app/{id}/with-user | 
*AppApi* | [**run**](docs/AppApi.md#run) | **POST** /api/app/app/run | 
*AppApi* | [**updateApp**](docs/AppApi.md#updateapp) | **PUT** /api/app/app/{id} | 
*AppApi* | [**updateRunState**](docs/AppApi.md#updaterunstate) | **PUT** /api/app/app/{id}/run-state | 
*AppAssetApi* | [**createAppAsset**](docs/AppAssetApi.md#createappasset) | **POST** /api/app/app-asset | 
*AppAssetApi* | [**deleteAppAssetById**](docs/AppAssetApi.md#deleteappassetbyid) | **DELETE** /api/app/app-asset/{id} | 
*AppAssetApi* | [**getListByAppLocaleId**](docs/AppAssetApi.md#getlistbyapplocaleid) | **GET** /api/app/app-asset/by-app-locale-id/{appLocaleId} | 
*AppAssetApi* | [**updateAppAsset**](docs/AppAssetApi.md#updateappasset) | **PUT** /api/app/app-asset/{id} | 
*AppFeatureApi* | [**createAppFeature**](docs/AppFeatureApi.md#createappfeature) | **POST** /api/app/app-feature | 
*AppFeatureApi* | [**deleteAppFeatureById**](docs/AppFeatureApi.md#deleteappfeaturebyid) | **DELETE** /api/app/app-feature/{id} | 
*AppFeatureApi* | [**getAppFeatureList**](docs/AppFeatureApi.md#getappfeaturelist) | **GET** /api/app/app-feature | 
*AppFeatureApi* | [**updateAppFeature**](docs/AppFeatureApi.md#updateappfeature) | **PUT** /api/app/app-feature/{id} | 
*AppFeedbackApi* | [**createAppFeedback**](docs/AppFeedbackApi.md#createappfeedback) | **POST** /api/app/app-feedback | 创建反馈（允许匿名用户提交）
*AppFeedbackApi* | [**deleteAppFeedbackById**](docs/AppFeedbackApi.md#deleteappfeedbackbyid) | **DELETE** /api/app/app-feedback/{id} | 
*AppFeedbackApi* | [**getAppFeedbackById**](docs/AppFeedbackApi.md#getappfeedbackbyid) | **GET** /api/app/app-feedback/{id} | 
*AppFeedbackApi* | [**getAppFeedbackList**](docs/AppFeedbackApi.md#getappfeedbacklist) | **GET** /api/app/app-feedback | 
*AppFeedbackApi* | [**markAsProcessed**](docs/AppFeedbackApi.md#markasprocessed) | **POST** /api/app/app-feedback/{id}/mark-as-processed | 
*AppFeedbackApi* | [**reply**](docs/AppFeedbackApi.md#reply) | **POST** /api/app/app-feedback/{id}/reply | 
*AppLocaleApi* | [**createAppLocale**](docs/AppLocaleApi.md#createapplocale) | **POST** /api/app/app-locale | 
*AppLocaleApi* | [**deleteAppLocaleById**](docs/AppLocaleApi.md#deleteapplocalebyid) | **DELETE** /api/app/app-locale/{id} | 
*AppLocaleApi* | [**getListByAppId**](docs/AppLocaleApi.md#getlistbyappid) | **GET** /api/app/app-locale/by-app-id/{appId} | 
*AppLocaleApi* | [**updateAppLocale**](docs/AppLocaleApi.md#updateapplocale) | **PUT** /api/app/app-locale/{id} | 
*AppPricingApi* | [**createAppPricing**](docs/AppPricingApi.md#createapppricing) | **POST** /api/app/app-pricing | 
*AppPricingApi* | [**deleteAppPricingById**](docs/AppPricingApi.md#deleteapppricingbyid) | **DELETE** /api/app/app-pricing/{id} | 
*AppPricingApi* | [**getAppPricingById**](docs/AppPricingApi.md#getapppricingbyid) | **GET** /api/app/app-pricing/{id} | 
*AppPricingApi* | [**getAppPricingList**](docs/AppPricingApi.md#getapppricinglist) | **GET** /api/app/app-pricing | 
*AppPricingApi* | [**getListByAppId**](docs/AppPricingApi.md#getlistbyappid) | **GET** /api/app/app-pricing/by-app-id/{appId} | 获取应用定价方案列表，允许匿名访问供未登录用户查看订阅计划
*AppPricingApi* | [**getPricingItemsByAppId**](docs/AppPricingApi.md#getpricingitemsbyappid) | **GET** /api/app/app-pricing/pricing-items-by-app-id/{appId} | 
*AppPricingApi* | [**updateAppPricing**](docs/AppPricingApi.md#updateapppricing) | **PUT** /api/app/app-pricing/{id} | 
*AppPricingItemApi* | [**createAppPricingItem**](docs/AppPricingItemApi.md#createapppricingitem) | **POST** /api/app/app-pricing-item | 
*AppPricingItemApi* | [**deleteAppPricingItemById**](docs/AppPricingItemApi.md#deleteapppricingitembyid) | **DELETE** /api/app/app-pricing-item/{id} | 
*AppPricingItemApi* | [**getAppPricingItemById**](docs/AppPricingItemApi.md#getapppricingitembyid) | **GET** /api/app/app-pricing-item/{id} | 
*AppPricingItemApi* | [**getAppPricingItemList**](docs/AppPricingItemApi.md#getapppricingitemlist) | **GET** /api/app/app-pricing-item | 
*AppPricingItemApi* | [**updateAppPricingItem**](docs/AppPricingItemApi.md#updateapppricingitem) | **PUT** /api/app/app-pricing-item/{id} | 
*AppReleaseApi* | [**createAppRelease**](docs/AppReleaseApi.md#createapprelease) | **POST** /api/app/app-release | 创建新版本
*AppReleaseApi* | [**deleteAppReleaseById**](docs/AppReleaseApi.md#deleteappreleasebyid) | **DELETE** /api/app/app-release/{id} | 删除版本
*AppReleaseApi* | [**getAppReleaseById**](docs/AppReleaseApi.md#getappreleasebyid) | **GET** /api/app/app-release/{id} | 获取版本
*AppReleaseApi* | [**getAppReleaseList**](docs/AppReleaseApi.md#getappreleaselist) | **GET** /api/app/app-release | 获取版本列表
*AppReleaseApi* | [**getLatest**](docs/AppReleaseApi.md#getlatest) | **GET** /api/app/app-release/latest | 获取最新版本
*AppReleaseApi* | [**getListByDeveloper**](docs/AppReleaseApi.md#getlistbydeveloper) | **GET** /api/app/app-release/by-developer | 开发者获取版本列表（版本的创建者为当前用户）
*AppReleaseApi* | [**updateAppRelease**](docs/AppReleaseApi.md#updateapprelease) | **PUT** /api/app/app-release/{id} | 更新版本
*AppSdkApi* | [**createAppSdk**](docs/AppSdkApi.md#createappsdk) | **POST** /api/app/app-sdk | 
*AppSdkApi* | [**deleteAppSdkById**](docs/AppSdkApi.md#deleteappsdkbyid) | **DELETE** /api/app/app-sdk/{id} | 
*AppSdkApi* | [**getAppSdkList**](docs/AppSdkApi.md#getappsdklist) | **GET** /api/app/app-sdk | 
*AppSdkApi* | [**updateAppSdk**](docs/AppSdkApi.md#updateappsdk) | **PUT** /api/app/app-sdk/{id} | 
*AppTesterApi* | [**checkIsAppTester**](docs/AppTesterApi.md#checkisapptester) | **POST** /api/app/app-tester/check-is-app-tester | 检查用户是否是内测用户
*AppTesterApi* | [**createAppTester**](docs/AppTesterApi.md#createapptester) | **POST** /api/app/app-tester | 创建内测用户
*AppTesterApi* | [**deleteAppTesterById**](docs/AppTesterApi.md#deleteapptesterbyid) | **DELETE** /api/app/app-tester/{id} | 删除内测用户
*AppTesterApi* | [**getAppTesterById**](docs/AppTesterApi.md#getapptesterbyid) | **GET** /api/app/app-tester/{id} | 获取内测用户
*AppTesterApi* | [**getAppTesterList**](docs/AppTesterApi.md#getapptesterlist) | **GET** /api/app/app-tester | 获取内测用户列表
*AppTesterApi* | [**updateAppTester**](docs/AppTesterApi.md#updateapptester) | **PUT** /api/app/app-tester/{id} | 更新内测用户
*AppUserScoreApi* | [**createAppUserScore**](docs/AppUserScoreApi.md#createappuserscore) | **POST** /api/app/app-user-score | 
*AvatarApi* | [**createAvatar**](docs/AvatarApi.md#createavatar) | **POST** /api/app/avatar | 
*AvatarApi* | [**getCredentials**](docs/AvatarApi.md#getcredentials) | **GET** /api/app/avatar/credentials | 
*BuildRecordApi* | [**createBuildRecord**](docs/BuildRecordApi.md#createbuildrecord) | **POST** /api/app/build-record | 
*BuildRecordApi* | [**deleteBuildRecordById**](docs/BuildRecordApi.md#deletebuildrecordbyid) | **DELETE** /api/app/build-record/{id} | 
*BuildRecordApi* | [**getBuildRecordById**](docs/BuildRecordApi.md#getbuildrecordbyid) | **GET** /api/app/build-record/{id} | 
*BuildRecordApi* | [**getBuildRecordList**](docs/BuildRecordApi.md#getbuildrecordlist) | **GET** /api/app/build-record | 
*BuildRecordApi* | [**getByCiBuildId**](docs/BuildRecordApi.md#getbycibuildid) | **GET** /api/app/build-record/by-ci-build-id/{ciBuildId} | 
*BuildRecordApi* | [**getLatest**](docs/BuildRecordApi.md#getlatest) | **GET** /api/app/build-record/latest/{appId} | 
*BuildRecordApi* | [**markAsBuilding**](docs/BuildRecordApi.md#markasbuilding) | **POST** /api/app/build-record/{id}/mark-as-building | 
*BuildRecordApi* | [**markAsCanceled**](docs/BuildRecordApi.md#markascanceled) | **POST** /api/app/build-record/{id}/mark-as-canceled | 
*BuildRecordApi* | [**markAsFailed**](docs/BuildRecordApi.md#markasfailed) | **POST** /api/app/build-record/{id}/mark-as-failed | 
*BuildRecordApi* | [**markAsSucceeded**](docs/BuildRecordApi.md#markassucceeded) | **POST** /api/app/build-record/{id}/mark-as-succeeded | 
*BuildRecordApi* | [**updateBuildRecord**](docs/BuildRecordApi.md#updatebuildrecord) | **PUT** /api/app/build-record/{id} | 
*DeployRecordApi* | [**createDeployRecord**](docs/DeployRecordApi.md#createdeployrecord) | **POST** /api/app/deploy-record | 
*DeployRecordApi* | [**deleteDeployRecordById**](docs/DeployRecordApi.md#deletedeployrecordbyid) | **DELETE** /api/app/deploy-record/{id} | 
*DeployRecordApi* | [**getByCiDeployId**](docs/DeployRecordApi.md#getbycideployid) | **GET** /api/app/deploy-record/by-ci-deploy-id/{ciDeployId} | 
*DeployRecordApi* | [**getDeployRecordById**](docs/DeployRecordApi.md#getdeployrecordbyid) | **GET** /api/app/deploy-record/{id} | 
*DeployRecordApi* | [**getDeployRecordList**](docs/DeployRecordApi.md#getdeployrecordlist) | **GET** /api/app/deploy-record | 
*DeployRecordApi* | [**getLatest**](docs/DeployRecordApi.md#getlatest) | **GET** /api/app/deploy-record/latest/{appId} | 
*DeployRecordApi* | [**getListByBuildRecordId**](docs/DeployRecordApi.md#getlistbybuildrecordid) | **GET** /api/app/deploy-record/by-build-record-id/{buildRecordId} | 
*DeployRecordApi* | [**markAsCanceled**](docs/DeployRecordApi.md#markascanceled) | **POST** /api/app/deploy-record/{id}/mark-as-canceled | 
*DeployRecordApi* | [**markAsDeploying**](docs/DeployRecordApi.md#markasdeploying) | **POST** /api/app/deploy-record/{id}/mark-as-deploying | 
*DeployRecordApi* | [**markAsFailed**](docs/DeployRecordApi.md#markasfailed) | **POST** /api/app/deploy-record/{id}/mark-as-failed | 
*DeployRecordApi* | [**markAsSucceeded**](docs/DeployRecordApi.md#markassucceeded) | **POST** /api/app/deploy-record/{id}/mark-as-succeeded | 
*DeployRecordApi* | [**updateDeployRecord**](docs/DeployRecordApi.md#updatedeployrecord) | **PUT** /api/app/deploy-record/{id} | 
*DeviceApi* | [**bind**](docs/DeviceApi.md#bind) | **POST** /api/app/device/bind | 
*DeviceApi* | [**getByToken**](docs/DeviceApi.md#getbytoken) | **GET** /api/app/device/by-token | 
*DeviceApi* | [**getDeviceById**](docs/DeviceApi.md#getdevicebyid) | **GET** /api/app/device/{id} | 
*DeviceApi* | [**getDeviceList**](docs/DeviceApi.md#getdevicelist) | **GET** /api/app/device | 
*DeviceApi* | [**refreshDevice**](docs/DeviceApi.md#refreshdevice) | **POST** /api/app/device/refresh-device | 
*DeviceApi* | [**remove**](docs/DeviceApi.md#remove) | **DELETE** /api/app/device | 
*DynamicClaimsApi* | [**refresh**](docs/DynamicClaimsApi.md#refresh) | **POST** /api/account/dynamic-claims/refresh | 
*EmailSettingsApi* | [**getEmailSettings**](docs/EmailSettingsApi.md#getemailsettings) | **GET** /api/setting-management/emailing | 
*EmailSettingsApi* | [**sendTestEmail**](docs/EmailSettingsApi.md#sendtestemail) | **POST** /api/setting-management/emailing/send-test-email | 
*EmailSettingsApi* | [**updateEmailSettings**](docs/EmailSettingsApi.md#updateemailsettings) | **POST** /api/setting-management/emailing | 
*FeaturesApi* | [**deleteFeatures**](docs/FeaturesApi.md#deletefeatures) | **DELETE** /api/feature-management/features | 
*FeaturesApi* | [**getFeatures**](docs/FeaturesApi.md#getfeatures) | **GET** /api/feature-management/features | 
*FeaturesApi* | [**updateFeatures**](docs/FeaturesApi.md#updatefeatures) | **PUT** /api/feature-management/features | 
*MessageApi* | [**publish**](docs/MessageApi.md#publish) | **POST** /api/app/message/publish | 
*MessageApi* | [**recall**](docs/MessageApi.md#recall) | **POST** /api/app/message/recall | 
*MessageApi* | [**subscribe**](docs/MessageApi.md#subscribe) | **POST** /api/app/message/subscribe | 
*MessageApi* | [**unsubscribe**](docs/MessageApi.md#unsubscribe) | **POST** /api/app/message/unsubscribe | 
*MessageSourceApi* | [**createMessageSource**](docs/MessageSourceApi.md#createmessagesource) | **POST** /api/app/message-source | 
*MessageSourceApi* | [**deleteMessageSourceById**](docs/MessageSourceApi.md#deletemessagesourcebyid) | **DELETE** /api/app/message-source/{id} | 
*MessageSourceApi* | [**getMessageSourceById**](docs/MessageSourceApi.md#getmessagesourcebyid) | **GET** /api/app/message-source/{id} | 
*MessageSourceApi* | [**getMessageSourceList**](docs/MessageSourceApi.md#getmessagesourcelist) | **GET** /api/app/message-source | 
*MessageSourceApi* | [**updateMessageSource**](docs/MessageSourceApi.md#updatemessagesource) | **PUT** /api/app/message-source/{id} | 
*MessageSourceCategoryApi* | [**getMessageSourceCategoryList**](docs/MessageSourceCategoryApi.md#getmessagesourcecategorylist) | **GET** /api/app/message-source-category | 
*MessageSourceRouteApi* | [**createMessageSourceRoute**](docs/MessageSourceRouteApi.md#createmessagesourceroute) | **POST** /api/app/message-source-route | 
*MessageSourceRouteApi* | [**deleteMessageSourceRouteById**](docs/MessageSourceRouteApi.md#deletemessagesourceroutebyid) | **DELETE** /api/app/message-source-route/{id} | 
*MessageSourceRouteApi* | [**getMessageSourceRouteById**](docs/MessageSourceRouteApi.md#getmessagesourceroutebyid) | **GET** /api/app/message-source-route/{id} | 
*MessageSourceRouteApi* | [**getMessageSourceRouteList**](docs/MessageSourceRouteApi.md#getmessagesourceroutelist) | **GET** /api/app/message-source-route | 
*MessageSourceRouteApi* | [**updateMessageSourceRoute**](docs/MessageSourceRouteApi.md#updatemessagesourceroute) | **PUT** /api/app/message-source-route/{id} | 
*MessageSourceRouteSubApi* | [**createMessageSourceRouteSub**](docs/MessageSourceRouteSubApi.md#createmessagesourceroutesub) | **POST** /api/app/message-source-route-sub | 
*MessageSourceRouteSubApi* | [**deleteMessageSourceRouteSubById**](docs/MessageSourceRouteSubApi.md#deletemessagesourceroutesubbyid) | **DELETE** /api/app/message-source-route-sub/{id} | 
*MessageSourceRouteSubApi* | [**getMessageSourceRouteSubById**](docs/MessageSourceRouteSubApi.md#getmessagesourceroutesubbyid) | **GET** /api/app/message-source-route-sub/{id} | 
*MessageSourceRouteSubApi* | [**getMessageSourceRouteSubList**](docs/MessageSourceRouteSubApi.md#getmessagesourceroutesublist) | **GET** /api/app/message-source-route-sub | 
*MessageSourceRouteSubApi* | [**updateMessageSourceRouteSub**](docs/MessageSourceRouteSubApi.md#updatemessagesourceroutesub) | **PUT** /api/app/message-source-route-sub/{id} | 
*MessageTemplateApi* | [**createMessageTemplate**](docs/MessageTemplateApi.md#createmessagetemplate) | **POST** /api/app/message-template | 
*MessageTemplateApi* | [**deleteMessageTemplateById**](docs/MessageTemplateApi.md#deletemessagetemplatebyid) | **DELETE** /api/app/message-template/{id} | 
*MessageTemplateApi* | [**getMessageTemplateById**](docs/MessageTemplateApi.md#getmessagetemplatebyid) | **GET** /api/app/message-template/{id} | 
*MessageTemplateApi* | [**getMessageTemplateList**](docs/MessageTemplateApi.md#getmessagetemplatelist) | **GET** /api/app/message-template | 
*MessageTemplateApi* | [**updateMessageTemplate**](docs/MessageTemplateApi.md#updatemessagetemplate) | **PUT** /api/app/message-template/{id} | 
*MessageTemplateReleaseApi* | [**createMessageTemplateRelease**](docs/MessageTemplateReleaseApi.md#createmessagetemplaterelease) | **POST** /api/app/message-template-release | 
*MessageTemplateReleaseApi* | [**getMessageTemplateReleaseById**](docs/MessageTemplateReleaseApi.md#getmessagetemplatereleasebyid) | **GET** /api/app/message-template-release/{id} | 
*MessageTemplateReleaseApi* | [**getMessageTemplateReleaseList**](docs/MessageTemplateReleaseApi.md#getmessagetemplatereleaselist) | **GET** /api/app/message-template-release | 
*NotificationApi* | [**bark**](docs/NotificationApi.md#bark) | **GET** /api/app/notification/bark/{apiKey}/{message} | Bark 推送，兼容 Bark 推送协议  TODO: 验证 API KEY 功能, 添加[个人访问令牌]功能
*NotificationApi* | [**getNotificationList**](docs/NotificationApi.md#getnotificationlist) | **GET** /api/app/notification | 
*NotificationApi* | [**push**](docs/NotificationApi.md#push) | **POST** /api/app/notification/push | 
*PermissionsApi* | [**getPermissions**](docs/PermissionsApi.md#getpermissions) | **GET** /api/permission-management/permissions | 
*PermissionsApi* | [**updatePermissions**](docs/PermissionsApi.md#updatepermissions) | **PUT** /api/permission-management/permissions | 
*ProfileApi* | [**changePassword**](docs/ProfileApi.md#changepassword) | **POST** /api/account/my-profile/change-password | 
*ProfileApi* | [**getProfile**](docs/ProfileApi.md#getprofile) | **GET** /api/account/my-profile | 
*ProfileApi* | [**updateProfile**](docs/ProfileApi.md#updateprofile) | **PUT** /api/account/my-profile | 
*RoleApi* | [**createIdentityRole**](docs/RoleApi.md#createidentityrole) | **POST** /api/identity/roles | 
*RoleApi* | [**deleteIdentityRoleById**](docs/RoleApi.md#deleteidentityrolebyid) | **DELETE** /api/identity/roles/{id} | 
*RoleApi* | [**getAllList**](docs/RoleApi.md#getalllist) | **GET** /api/identity/roles/all | 
*RoleApi* | [**getIdentityRoleById**](docs/RoleApi.md#getidentityrolebyid) | **GET** /api/identity/roles/{id} | 
*RoleApi* | [**getIdentityRoleList**](docs/RoleApi.md#getidentityrolelist) | **GET** /api/identity/roles | 
*RoleApi* | [**updateIdentityRole**](docs/RoleApi.md#updateidentityrole) | **PUT** /api/identity/roles/{id} | 
*StorageObjectApi* | [**getCdnDomains**](docs/StorageObjectApi.md#getcdndomains) | **GET** /api/app/storage-object/cdn-domains | 获取所有 CDN Domain 配置
*StorageObjectApi* | [**getFileCredential**](docs/StorageObjectApi.md#getfilecredential) | **GET** /api/app/storage-object/file-credential | 
*StorageObjectApi* | [**getUserStorages**](docs/StorageObjectApi.md#getuserstorages) | **GET** /api/app/storage-object/user-storages | 
*StorageObjectApi* | [**preSignUrl**](docs/StorageObjectApi.md#presignurl) | **POST** /api/app/storage-object/pre-sign-url | 
*SubscriptionApi* | [**appleNotifications**](docs/SubscriptionApi.md#applenotifications) | **POST** /api/app/subscription/apple-notifications | 苹果订阅 Callback 地址
*SubscriptionApi* | [**capturePayPalOrder**](docs/SubscriptionApi.md#capturepaypalorder) | **POST** /api/app/subscription/capture-pay-pal-order | 捕获 PayPal 订单并完成订阅
*SubscriptionApi* | [**createOrder**](docs/SubscriptionApi.md#createorder) | **POST** /api/app/subscription/order | 
*SubscriptionApi* | [**createPayPalOrder**](docs/SubscriptionApi.md#createpaypalorder) | **POST** /api/app/subscription/pay-pal-order | 创建 PayPal 订单
*SubscriptionApi* | [**getSubscriptionById**](docs/SubscriptionApi.md#getsubscriptionbyid) | **GET** /api/app/subscription | 
*SubscriptionApi* | [**getSubscriptionList**](docs/SubscriptionApi.md#getsubscriptionlist) | **GET** /api/app/subscription/list | 获取用户订阅列表，每个应用只返回最新的一条订阅记录（含有效和已过期的）
*SubscriptionApi* | [**verifyReceipt**](docs/SubscriptionApi.md#verifyreceipt) | **POST** /api/app/subscription/verify-receipt | 
*TenantApi* | [**createTenant**](docs/TenantApi.md#createtenant) | **POST** /api/multi-tenancy/tenants | 
*TenantApi* | [**deleteDefaultConnectionString**](docs/TenantApi.md#deletedefaultconnectionstring) | **DELETE** /api/multi-tenancy/tenants/{id}/default-connection-string | 
*TenantApi* | [**deleteTenantById**](docs/TenantApi.md#deletetenantbyid) | **DELETE** /api/multi-tenancy/tenants/{id} | 
*TenantApi* | [**getDefaultConnectionString**](docs/TenantApi.md#getdefaultconnectionstring) | **GET** /api/multi-tenancy/tenants/{id}/default-connection-string | 
*TenantApi* | [**getTenantById**](docs/TenantApi.md#gettenantbyid) | **GET** /api/multi-tenancy/tenants/{id} | 
*TenantApi* | [**getTenantList**](docs/TenantApi.md#gettenantlist) | **GET** /api/multi-tenancy/tenants | 
*TenantApi* | [**updateDefaultConnectionString**](docs/TenantApi.md#updatedefaultconnectionstring) | **PUT** /api/multi-tenancy/tenants/{id}/default-connection-string | 
*TenantApi* | [**updateTenant**](docs/TenantApi.md#updatetenant) | **PUT** /api/multi-tenancy/tenants/{id} | 
*TimeZoneSettingsApi* | [**getTimeZoneSettings**](docs/TimeZoneSettingsApi.md#gettimezonesettings) | **GET** /api/setting-management/timezone | 
*TimeZoneSettingsApi* | [**getTimezones**](docs/TimeZoneSettingsApi.md#gettimezones) | **GET** /api/setting-management/timezone/timezones | 
*TimeZoneSettingsApi* | [**updateTimeZoneSettings**](docs/TimeZoneSettingsApi.md#updatetimezonesettings) | **POST** /api/setting-management/timezone | 
*UserApi* | [**createIdentityUser**](docs/UserApi.md#createidentityuser) | **POST** /api/identity/users | 
*UserApi* | [**deleteIdentityUserById**](docs/UserApi.md#deleteidentityuserbyid) | **DELETE** /api/identity/users/{id} | 
*UserApi* | [**findByEmail**](docs/UserApi.md#findbyemail) | **GET** /api/identity/users/by-email/{email} | 
*UserApi* | [**findByUsername**](docs/UserApi.md#findbyusername) | **GET** /api/identity/users/by-username/{userName} | 
*UserApi* | [**getAssignableRoles**](docs/UserApi.md#getassignableroles) | **GET** /api/identity/users/assignable-roles | 
*UserApi* | [**getIdentityUserById**](docs/UserApi.md#getidentityuserbyid) | **GET** /api/identity/users/{id} | 
*UserApi* | [**getIdentityUserList**](docs/UserApi.md#getidentityuserlist) | **GET** /api/identity/users | 
*UserApi* | [**getRoles**](docs/UserApi.md#getroles) | **GET** /api/identity/users/{id}/roles | 
*UserApi* | [**updateIdentityUser**](docs/UserApi.md#updateidentityuser) | **PUT** /api/identity/users/{id} | 
*UserApi* | [**updateRoles**](docs/UserApi.md#updateroles) | **PUT** /api/identity/users/{id}/roles | 
*UserLookupApi* | [**findById**](docs/UserLookupApi.md#findbyid) | **GET** /api/identity/users/lookup/{id} | 
*UserLookupApi* | [**findByUserName**](docs/UserLookupApi.md#findbyusername) | **GET** /api/identity/users/lookup/by-username/{userName} | 
*UserLookupApi* | [**getCount**](docs/UserLookupApi.md#getcount) | **GET** /api/identity/users/lookup/count | 
*UserLookupApi* | [**search**](docs/UserLookupApi.md#search) | **GET** /api/identity/users/lookup/search | 
*VerificationApi* | [**sendCode**](docs/VerificationApi.md#sendcode) | **POST** /api/app/verification/send-code | 
*VerificationApi* | [**sendCodeAnonymous**](docs/VerificationApi.md#sendcodeanonymous) | **POST** /api/app/verification/send-code-anonymous | 


### Documentation For Models

 - [AccountDeletionDto](docs/AccountDeletionDto.md)
 - [ActionApiDescriptionModel](docs/ActionApiDescriptionModel.md)
 - [ApiKeyCreateDto](docs/ApiKeyCreateDto.md)
 - [ApiKeyDto](docs/ApiKeyDto.md)
 - [ApiKeyDtoPagedResultDto](docs/ApiKeyDtoPagedResultDto.md)
 - [ApiKeyUpdateDto](docs/ApiKeyUpdateDto.md)
 - [AppAssetDeviceType](docs/AppAssetDeviceType.md)
 - [AppAssetDto](docs/AppAssetDto.md)
 - [AppAssetType](docs/AppAssetType.md)
 - [AppDto](docs/AppDto.md)
 - [AppDtoPagedResultDto](docs/AppDtoPagedResultDto.md)
 - [AppFeatureDto](docs/AppFeatureDto.md)
 - [AppFeatureDtoPagedResultDto](docs/AppFeatureDtoPagedResultDto.md)
 - [AppFeatureLocaleDto](docs/AppFeatureLocaleDto.md)
 - [AppFeedbackDto](docs/AppFeedbackDto.md)
 - [AppFeedbackDtoPagedResultDto](docs/AppFeedbackDtoPagedResultDto.md)
 - [AppFeedbackStatus](docs/AppFeedbackStatus.md)
 - [AppFeedbackType](docs/AppFeedbackType.md)
 - [AppFramework](docs/AppFramework.md)
 - [AppLocaleDto](docs/AppLocaleDto.md)
 - [AppPlatform](docs/AppPlatform.md)
 - [AppPriceNaming](docs/AppPriceNaming.md)
 - [AppPricingDto](docs/AppPricingDto.md)
 - [AppPricingDtoPagedResultDto](docs/AppPricingDtoPagedResultDto.md)
 - [AppPricingItemDto](docs/AppPricingItemDto.md)
 - [AppPricingItemValueDto](docs/AppPricingItemValueDto.md)
 - [AppPublisher](docs/AppPublisher.md)
 - [AppReleaseDto](docs/AppReleaseDto.md)
 - [AppReleaseDtoPagedResultDto](docs/AppReleaseDtoPagedResultDto.md)
 - [AppRunDto](docs/AppRunDto.md)
 - [AppRunRecordDto](docs/AppRunRecordDto.md)
 - [AppRunRecordUpdateDto](docs/AppRunRecordUpdateDto.md)
 - [AppRunStatus](docs/AppRunStatus.md)
 - [AppSdkDto](docs/AppSdkDto.md)
 - [AppSdkDtoPagedResultDto](docs/AppSdkDtoPagedResultDto.md)
 - [AppTesterDto](docs/AppTesterDto.md)
 - [AppTesterDtoPagedResultDto](docs/AppTesterDtoPagedResultDto.md)
 - [AppType](docs/AppType.md)
 - [AppUserScoreDto](docs/AppUserScoreDto.md)
 - [AppWithUserDto](docs/AppWithUserDto.md)
 - [AppWithUserDtoPagedResultDto](docs/AppWithUserDtoPagedResultDto.md)
 - [AppleNotificaionDto](docs/AppleNotificaionDto.md)
 - [AppleVerifyReceiptResult](docs/AppleVerifyReceiptResult.md)
 - [ApplicationApiDescriptionModel](docs/ApplicationApiDescriptionModel.md)
 - [ApplicationAuthConfigurationDto](docs/ApplicationAuthConfigurationDto.md)
 - [ApplicationConfigurationDto](docs/ApplicationConfigurationDto.md)
 - [ApplicationFeatureConfigurationDto](docs/ApplicationFeatureConfigurationDto.md)
 - [ApplicationGlobalFeatureConfigurationDto](docs/ApplicationGlobalFeatureConfigurationDto.md)
 - [ApplicationLocalizationConfigurationDto](docs/ApplicationLocalizationConfigurationDto.md)
 - [ApplicationLocalizationDto](docs/ApplicationLocalizationDto.md)
 - [ApplicationLocalizationResourceDto](docs/ApplicationLocalizationResourceDto.md)
 - [ApplicationSettingConfigurationDto](docs/ApplicationSettingConfigurationDto.md)
 - [ArtifactType](docs/ArtifactType.md)
 - [AvatarDto](docs/AvatarDto.md)
 - [BindDeviceDto](docs/BindDeviceDto.md)
 - [BuildRecordDto](docs/BuildRecordDto.md)
 - [BuildRecordDtoPagedResultDto](docs/BuildRecordDtoPagedResultDto.md)
 - [BuildStatus](docs/BuildStatus.md)
 - [BuildTrigger](docs/BuildTrigger.md)
 - [CapturePayPalOrderDto](docs/CapturePayPalOrderDto.md)
 - [CdnDomainDto](docs/CdnDomainDto.md)
 - [ChangePasswordDto](docs/ChangePasswordDto.md)
 - [ChangePasswordInput](docs/ChangePasswordInput.md)
 - [CheckSyncAuthResultDto](docs/CheckSyncAuthResultDto.md)
 - [ClockDto](docs/ClockDto.md)
 - [ControllerApiDescriptionModel](docs/ControllerApiDescriptionModel.md)
 - [ControllerInterfaceApiDescriptionModel](docs/ControllerInterfaceApiDescriptionModel.md)
 - [CreateAppFeedbackDto](docs/CreateAppFeedbackDto.md)
 - [CreateAvatarDto](docs/CreateAvatarDto.md)
 - [CreateBuildRecordDto](docs/CreateBuildRecordDto.md)
 - [CreateDeployRecordDto](docs/CreateDeployRecordDto.md)
 - [CreateMessageTemplateReleaseDto](docs/CreateMessageTemplateReleaseDto.md)
 - [CreateOpenIddictApplicationDto](docs/CreateOpenIddictApplicationDto.md)
 - [CreateOrGetSubscriptionOrderDto](docs/CreateOrGetSubscriptionOrderDto.md)
 - [CreateOrUpdateAppAssetDto](docs/CreateOrUpdateAppAssetDto.md)
 - [CreateOrUpdateAppDto](docs/CreateOrUpdateAppDto.md)
 - [CreateOrUpdateAppFeatureDto](docs/CreateOrUpdateAppFeatureDto.md)
 - [CreateOrUpdateAppFeatureLocaleDto](docs/CreateOrUpdateAppFeatureLocaleDto.md)
 - [CreateOrUpdateAppLocaleDto](docs/CreateOrUpdateAppLocaleDto.md)
 - [CreateOrUpdateAppPricingDto](docs/CreateOrUpdateAppPricingDto.md)
 - [CreateOrUpdateAppPricingItemDto](docs/CreateOrUpdateAppPricingItemDto.md)
 - [CreateOrUpdateAppReleaseDto](docs/CreateOrUpdateAppReleaseDto.md)
 - [CreateOrUpdateAppSdkDto](docs/CreateOrUpdateAppSdkDto.md)
 - [CreateOrUpdateAppUserScoreDto](docs/CreateOrUpdateAppUserScoreDto.md)
 - [CreateOrUpdateMessageTemplateDto](docs/CreateOrUpdateMessageTemplateDto.md)
 - [CreatePayPalOrderDto](docs/CreatePayPalOrderDto.md)
 - [CreatePayPalOrderResultDto](docs/CreatePayPalOrderResultDto.md)
 - [CreatePushNotificationDto](docs/CreatePushNotificationDto.md)
 - [CreateUpdateAppTesterDto](docs/CreateUpdateAppTesterDto.md)
 - [CreateUpdateMessageSourceDto](docs/CreateUpdateMessageSourceDto.md)
 - [CreateUpdateMessageSourceRouteDto](docs/CreateUpdateMessageSourceRouteDto.md)
 - [CreateUpdateMessageSourceRouteSubDto](docs/CreateUpdateMessageSourceRouteSubDto.md)
 - [CurrentCultureDto](docs/CurrentCultureDto.md)
 - [CurrentTenantDto](docs/CurrentTenantDto.md)
 - [CurrentUserDto](docs/CurrentUserDto.md)
 - [DateTimeFormatDto](docs/DateTimeFormatDto.md)
 - [DeployRecordDto](docs/DeployRecordDto.md)
 - [DeployRecordDtoPagedResultDto](docs/DeployRecordDtoPagedResultDto.md)
 - [DeployStatus](docs/DeployStatus.md)
 - [DeviceDto](docs/DeviceDto.md)
 - [DeviceDtoPagedResultDto](docs/DeviceDtoPagedResultDto.md)
 - [DeviceStatus](docs/DeviceStatus.md)
 - [EmailSettingsDto](docs/EmailSettingsDto.md)
 - [EntityExtensionDto](docs/EntityExtensionDto.md)
 - [ExtensionEnumDto](docs/ExtensionEnumDto.md)
 - [ExtensionEnumFieldDto](docs/ExtensionEnumFieldDto.md)
 - [ExtensionPropertyApiCreateDto](docs/ExtensionPropertyApiCreateDto.md)
 - [ExtensionPropertyApiDto](docs/ExtensionPropertyApiDto.md)
 - [ExtensionPropertyApiGetDto](docs/ExtensionPropertyApiGetDto.md)
 - [ExtensionPropertyApiUpdateDto](docs/ExtensionPropertyApiUpdateDto.md)
 - [ExtensionPropertyAttributeDto](docs/ExtensionPropertyAttributeDto.md)
 - [ExtensionPropertyDto](docs/ExtensionPropertyDto.md)
 - [ExtensionPropertyUiDto](docs/ExtensionPropertyUiDto.md)
 - [ExtensionPropertyUiFormDto](docs/ExtensionPropertyUiFormDto.md)
 - [ExtensionPropertyUiLookupDto](docs/ExtensionPropertyUiLookupDto.md)
 - [ExtensionPropertyUiTableDto](docs/ExtensionPropertyUiTableDto.md)
 - [FeatureDto](docs/FeatureDto.md)
 - [FeatureGroupDto](docs/FeatureGroupDto.md)
 - [FeatureProviderDto](docs/FeatureProviderDto.md)
 - [FindTenantResultDto](docs/FindTenantResultDto.md)
 - [GetFeatureListResultDto](docs/GetFeatureListResultDto.md)
 - [GetPermissionListResultDto](docs/GetPermissionListResultDto.md)
 - [GitRepositoryType](docs/GitRepositoryType.md)
 - [IStringValueType](docs/IStringValueType.md)
 - [IValueValidator](docs/IValueValidator.md)
 - [IanaTimeZone](docs/IanaTimeZone.md)
 - [IdentityRoleCreateDto](docs/IdentityRoleCreateDto.md)
 - [IdentityRoleDto](docs/IdentityRoleDto.md)
 - [IdentityRoleDtoListResultDto](docs/IdentityRoleDtoListResultDto.md)
 - [IdentityRoleDtoPagedResultDto](docs/IdentityRoleDtoPagedResultDto.md)
 - [IdentityRoleUpdateDto](docs/IdentityRoleUpdateDto.md)
 - [IdentityUser](docs/IdentityUser.md)
 - [IdentityUserClaim](docs/IdentityUserClaim.md)
 - [IdentityUserCreateDto](docs/IdentityUserCreateDto.md)
 - [IdentityUserDto](docs/IdentityUserDto.md)
 - [IdentityUserDtoPagedResultDto](docs/IdentityUserDtoPagedResultDto.md)
 - [IdentityUserLogin](docs/IdentityUserLogin.md)
 - [IdentityUserOrganizationUnit](docs/IdentityUserOrganizationUnit.md)
 - [IdentityUserRole](docs/IdentityUserRole.md)
 - [IdentityUserToken](docs/IdentityUserToken.md)
 - [IdentityUserUpdateDto](docs/IdentityUserUpdateDto.md)
 - [IdentityUserUpdateRolesDto](docs/IdentityUserUpdateRolesDto.md)
 - [InApp](docs/InApp.md)
 - [InterfaceMethodApiDescriptionModel](docs/InterfaceMethodApiDescriptionModel.md)
 - [LanguageInfo](docs/LanguageInfo.md)
 - [LatestReceiptInfo](docs/LatestReceiptInfo.md)
 - [LocalizableStringDto](docs/LocalizableStringDto.md)
 - [MessagePublishDto](docs/MessagePublishDto.md)
 - [MessageRecallDto](docs/MessageRecallDto.md)
 - [MessageSourceCategoryDto](docs/MessageSourceCategoryDto.md)
 - [MessageSourceDto](docs/MessageSourceDto.md)
 - [MessageSourceRouteDto](docs/MessageSourceRouteDto.md)
 - [MessageSourceRouteSubDto](docs/MessageSourceRouteSubDto.md)
 - [MessageSubscribeDto](docs/MessageSubscribeDto.md)
 - [MessageTemplateDto](docs/MessageTemplateDto.md)
 - [MessageTemplateReleaseDto](docs/MessageTemplateReleaseDto.md)
 - [MessageUnsubscribeDto](docs/MessageUnsubscribeDto.md)
 - [MethodParameterApiDescriptionModel](docs/MethodParameterApiDescriptionModel.md)
 - [ModuleApiDescriptionModel](docs/ModuleApiDescriptionModel.md)
 - [ModuleExtensionDto](docs/ModuleExtensionDto.md)
 - [MultiTenancyInfoDto](docs/MultiTenancyInfoDto.md)
 - [NameValue](docs/NameValue.md)
 - [NotificationInfoDto](docs/NotificationInfoDto.md)
 - [NotificationInfoDtoPagedResultDto](docs/NotificationInfoDtoPagedResultDto.md)
 - [ObjectExtensionsDto](docs/ObjectExtensionsDto.md)
 - [ParameterApiDescriptionModel](docs/ParameterApiDescriptionModel.md)
 - [PendingRenewalInfo](docs/PendingRenewalInfo.md)
 - [PermissionGrantInfoDto](docs/PermissionGrantInfoDto.md)
 - [PermissionGroupDto](docs/PermissionGroupDto.md)
 - [ProfileDto](docs/ProfileDto.md)
 - [PropertyApiDescriptionModel](docs/PropertyApiDescriptionModel.md)
 - [ProviderInfoDto](docs/ProviderInfoDto.md)
 - [Receipt](docs/Receipt.md)
 - [RefreshDeviceStatusDto](docs/RefreshDeviceStatusDto.md)
 - [RegisterDto](docs/RegisterDto.md)
 - [ReleaseChannel](docs/ReleaseChannel.md)
 - [RemoteServiceErrorInfo](docs/RemoteServiceErrorInfo.md)
 - [RemoteServiceErrorResponse](docs/RemoteServiceErrorResponse.md)
 - [RemoteServiceValidationErrorInfo](docs/RemoteServiceValidationErrorInfo.md)
 - [ReplyAppFeedbackDto](docs/ReplyAppFeedbackDto.md)
 - [ResetPasswordDto](docs/ResetPasswordDto.md)
 - [ReturnValueApiDescriptionModel](docs/ReturnValueApiDescriptionModel.md)
 - [SendPasswordResetCodeDto](docs/SendPasswordResetCodeDto.md)
 - [SendTestEmailInput](docs/SendTestEmailInput.md)
 - [SendVerificationCodeDto](docs/SendVerificationCodeDto.md)
 - [StorageObjectCredentials](docs/StorageObjectCredentials.md)
 - [SubscriptionDto](docs/SubscriptionDto.md)
 - [SubscriptionOrderDto](docs/SubscriptionOrderDto.md)
 - [SubscriptionOrderStatus](docs/SubscriptionOrderStatus.md)
 - [SubscriptionOrderType](docs/SubscriptionOrderType.md)
 - [TenantCreateDto](docs/TenantCreateDto.md)
 - [TenantDto](docs/TenantDto.md)
 - [TenantDtoPagedResultDto](docs/TenantDtoPagedResultDto.md)
 - [TenantUpdateDto](docs/TenantUpdateDto.md)
 - [TimeZone](docs/TimeZone.md)
 - [TimingDto](docs/TimingDto.md)
 - [TypeApiDescriptionModel](docs/TypeApiDescriptionModel.md)
 - [UpdateBuildRecordDto](docs/UpdateBuildRecordDto.md)
 - [UpdateDeployRecordDto](docs/UpdateDeployRecordDto.md)
 - [UpdateEmailSettingsDto](docs/UpdateEmailSettingsDto.md)
 - [UpdateFeatureDto](docs/UpdateFeatureDto.md)
 - [UpdateFeaturesDto](docs/UpdateFeaturesDto.md)
 - [UpdatePermissionDto](docs/UpdatePermissionDto.md)
 - [UpdatePermissionsDto](docs/UpdatePermissionsDto.md)
 - [UpdateProfileDto](docs/UpdateProfileDto.md)
 - [UserData](docs/UserData.md)
 - [UserDataListResultDto](docs/UserDataListResultDto.md)
 - [UserProfileDto](docs/UserProfileDto.md)
 - [UserStorageDto](docs/UserStorageDto.md)
 - [UserStorageItemDto](docs/UserStorageItemDto.md)
 - [VerifyPasswordResetTokenInput](docs/VerifyPasswordResetTokenInput.md)
 - [VerifyReceiptDto](docs/VerifyReceiptDto.md)
 - [VerifyReceiptResult](docs/VerifyReceiptResult.md)
 - [WindowsTimeZone](docs/WindowsTimeZone.md)


<a id="documentation-for-authorization"></a>
## Documentation For Authorization


Authentication schemes defined for the API:
<a id="oauth2"></a>
### oauth2

- **Type**: OAuth
- **Flow**: accessCode
- **Authorization URL**: https://localhost:44301/connect/authorize
- **Scopes**: 
 - **Puupees**: Puupees API

