# AuthApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**loginApiV1AuthLoginPost**](#loginapiv1authloginpost) | **POST** /api/v1/auth/login | Login|
|[**logoutApiV1AuthLogoutPost**](#logoutapiv1authlogoutpost) | **POST** /api/v1/auth/logout | Logout|
|[**refreshApiV1AuthRefreshPost**](#refreshapiv1authrefreshpost) | **POST** /api/v1/auth/refresh | Refresh|
|[**verifyApiV1AuthVerifyPost**](#verifyapiv1authverifypost) | **POST** /api/v1/auth/verify | Verify|

# **loginApiV1AuthLoginPost**
> loginApiV1AuthLoginPost(loginRequest)


### Example

```typescript
import {
    AuthApi,
    Configuration,
    LoginRequest
} from '@bianlat/api-client';

const configuration = new Configuration();
const apiInstance = new AuthApi(configuration);

let loginRequest: LoginRequest; //

const { status, data } = await apiInstance.loginApiV1AuthLoginPost(
    loginRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **loginRequest** | **LoginRequest**|  | |


### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **logoutApiV1AuthLogoutPost**
> logoutApiV1AuthLogoutPost(refreshRequest)


### Example

```typescript
import {
    AuthApi,
    Configuration,
    RefreshRequest
} from '@bianlat/api-client';

const configuration = new Configuration();
const apiInstance = new AuthApi(configuration);

let refreshRequest: RefreshRequest; //

const { status, data } = await apiInstance.logoutApiV1AuthLogoutPost(
    refreshRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **refreshRequest** | **RefreshRequest**|  | |


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

# **refreshApiV1AuthRefreshPost**
> TokenResponse refreshApiV1AuthRefreshPost(refreshRequest)


### Example

```typescript
import {
    AuthApi,
    Configuration,
    RefreshRequest
} from '@bianlat/api-client';

const configuration = new Configuration();
const apiInstance = new AuthApi(configuration);

let refreshRequest: RefreshRequest; //

const { status, data } = await apiInstance.refreshApiV1AuthRefreshPost(
    refreshRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **refreshRequest** | **RefreshRequest**|  | |


### Return type

**TokenResponse**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **verifyApiV1AuthVerifyPost**
> TokenResponse verifyApiV1AuthVerifyPost(verifyRequest)


### Example

```typescript
import {
    AuthApi,
    Configuration,
    VerifyRequest
} from '@bianlat/api-client';

const configuration = new Configuration();
const apiInstance = new AuthApi(configuration);

let verifyRequest: VerifyRequest; //

const { status, data } = await apiInstance.verifyApiV1AuthVerifyPost(
    verifyRequest
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **verifyRequest** | **VerifyRequest**|  | |


### Return type

**TokenResponse**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

