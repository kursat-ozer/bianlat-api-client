# NotificationsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**deleteDeviceTokenApiV1NotificationsDeviceTokensDelete**](#deletedevicetokenapiv1notificationsdevicetokensdelete) | **DELETE** /api/v1/notifications/device-tokens | Delete Device Token|
|[**registerDeviceTokenApiV1NotificationsDeviceTokensPost**](#registerdevicetokenapiv1notificationsdevicetokenspost) | **POST** /api/v1/notifications/device-tokens | Register Device Token|

# **deleteDeviceTokenApiV1NotificationsDeviceTokensDelete**
> deleteDeviceTokenApiV1NotificationsDeviceTokensDelete(deviceTokenDelete)


### Example

```typescript
import {
    NotificationsApi,
    Configuration,
    DeviceTokenDelete
} from '@bianlat/api-client';

const configuration = new Configuration();
const apiInstance = new NotificationsApi(configuration);

let deviceTokenDelete: DeviceTokenDelete; //

const { status, data } = await apiInstance.deleteDeviceTokenApiV1NotificationsDeviceTokensDelete(
    deviceTokenDelete
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **deviceTokenDelete** | **DeviceTokenDelete**|  | |


### Return type

void (empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **registerDeviceTokenApiV1NotificationsDeviceTokensPost**
> any registerDeviceTokenApiV1NotificationsDeviceTokensPost(deviceTokenRegister)


### Example

```typescript
import {
    NotificationsApi,
    Configuration,
    DeviceTokenRegister
} from '@bianlat/api-client';

const configuration = new Configuration();
const apiInstance = new NotificationsApi(configuration);

let deviceTokenRegister: DeviceTokenRegister; //

const { status, data } = await apiInstance.registerDeviceTokenApiV1NotificationsDeviceTokensPost(
    deviceTokenRegister
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **deviceTokenRegister** | **DeviceTokenRegister**|  | |


### Return type

**any**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**201** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

