# AuthApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**loginApiV1AuthLoginPost**](AuthApi.md#loginapiv1authloginpost) | **POST** /api/v1/auth/login | Login |
| [**logoutApiV1AuthLogoutPost**](AuthApi.md#logoutapiv1authlogoutpost) | **POST** /api/v1/auth/logout | Logout |
| [**refreshApiV1AuthRefreshPost**](AuthApi.md#refreshapiv1authrefreshpost) | **POST** /api/v1/auth/refresh | Refresh |
| [**verifyApiV1AuthVerifyPost**](AuthApi.md#verifyapiv1authverifypost) | **POST** /api/v1/auth/verify | Verify |



## loginApiV1AuthLoginPost

> loginApiV1AuthLoginPost(loginRequest)

Login

### Example

```ts
import {
  Configuration,
  AuthApi,
} from '@bianlat/api-client';
import type { LoginApiV1AuthLoginPostRequest } from '@bianlat/api-client';

async function example() {
  console.log("🚀 Testing @bianlat/api-client SDK...");
  const api = new AuthApi();

  const body = {
    // LoginRequest
    loginRequest: ...,
  } satisfies LoginApiV1AuthLoginPostRequest;

  try {
    const data = await api.loginApiV1AuthLoginPost(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **loginRequest** | [LoginRequest](LoginRequest.md) |  | |

### Return type

`void` (Empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## logoutApiV1AuthLogoutPost

> logoutApiV1AuthLogoutPost(refreshRequest)

Logout

### Example

```ts
import {
  Configuration,
  AuthApi,
} from '@bianlat/api-client';
import type { LogoutApiV1AuthLogoutPostRequest } from '@bianlat/api-client';

async function example() {
  console.log("🚀 Testing @bianlat/api-client SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthApi(config);

  const body = {
    // RefreshRequest
    refreshRequest: ...,
  } satisfies LogoutApiV1AuthLogoutPostRequest;

  try {
    const data = await api.logoutApiV1AuthLogoutPost(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **refreshRequest** | [RefreshRequest](RefreshRequest.md) |  | |

### Return type

`void` (Empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## refreshApiV1AuthRefreshPost

> TokenResponse refreshApiV1AuthRefreshPost(refreshRequest)

Refresh

### Example

```ts
import {
  Configuration,
  AuthApi,
} from '@bianlat/api-client';
import type { RefreshApiV1AuthRefreshPostRequest } from '@bianlat/api-client';

async function example() {
  console.log("🚀 Testing @bianlat/api-client SDK...");
  const api = new AuthApi();

  const body = {
    // RefreshRequest
    refreshRequest: ...,
  } satisfies RefreshApiV1AuthRefreshPostRequest;

  try {
    const data = await api.refreshApiV1AuthRefreshPost(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **refreshRequest** | [RefreshRequest](RefreshRequest.md) |  | |

### Return type

[**TokenResponse**](TokenResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## verifyApiV1AuthVerifyPost

> TokenResponse verifyApiV1AuthVerifyPost(verifyRequest)

Verify

### Example

```ts
import {
  Configuration,
  AuthApi,
} from '@bianlat/api-client';
import type { VerifyApiV1AuthVerifyPostRequest } from '@bianlat/api-client';

async function example() {
  console.log("🚀 Testing @bianlat/api-client SDK...");
  const api = new AuthApi();

  const body = {
    // VerifyRequest
    verifyRequest: ...,
  } satisfies VerifyApiV1AuthVerifyPostRequest;

  try {
    const data = await api.verifyApiV1AuthVerifyPost(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **verifyRequest** | [VerifyRequest](VerifyRequest.md) |  | |

### Return type

[**TokenResponse**](TokenResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

