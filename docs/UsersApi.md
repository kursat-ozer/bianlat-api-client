# UsersApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addContactApiV1UsersContactsPost**](UsersApi.md#addcontactapiv1userscontactspost) | **POST** /api/v1/users/contacts | Add Contact |
| [**getContactApiV1UsersContactsContactUserIdGet**](UsersApi.md#getcontactapiv1userscontactscontactuseridget) | **GET** /api/v1/users/contacts/{contact_user_id} | Get Contact |
| [**getMeApiV1UsersMeGet**](UsersApi.md#getmeapiv1usersmeget) | **GET** /api/v1/users/me | Get Me |
| [**listContactsApiV1UsersContactsGet**](UsersApi.md#listcontactsapiv1userscontactsget) | **GET** /api/v1/users/contacts | List Contacts |
| [**removeContactApiV1UsersContactsContactUserIdDelete**](UsersApi.md#removecontactapiv1userscontactscontactuseriddelete) | **DELETE** /api/v1/users/contacts/{contact_user_id} | Remove Contact |
| [**updateMeApiV1UsersMePatch**](UsersApi.md#updatemeapiv1usersmepatch) | **PATCH** /api/v1/users/me | Update Me |



## addContactApiV1UsersContactsPost

> ContactRead addContactApiV1UsersContactsPost(contactCreate)

Add Contact

### Example

```ts
import {
  Configuration,
  UsersApi,
} from '@bianlat/api-client';
import type { AddContactApiV1UsersContactsPostRequest } from '@bianlat/api-client';

async function example() {
  console.log("🚀 Testing @bianlat/api-client SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UsersApi(config);

  const body = {
    // ContactCreate
    contactCreate: ...,
  } satisfies AddContactApiV1UsersContactsPostRequest;

  try {
    const data = await api.addContactApiV1UsersContactsPost(body);
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
| **contactCreate** | [ContactCreate](ContactCreate.md) |  | |

### Return type

[**ContactRead**](ContactRead.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getContactApiV1UsersContactsContactUserIdGet

> ContactRead getContactApiV1UsersContactsContactUserIdGet(contactUserId)

Get Contact

### Example

```ts
import {
  Configuration,
  UsersApi,
} from '@bianlat/api-client';
import type { GetContactApiV1UsersContactsContactUserIdGetRequest } from '@bianlat/api-client';

async function example() {
  console.log("🚀 Testing @bianlat/api-client SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UsersApi(config);

  const body = {
    // string
    contactUserId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies GetContactApiV1UsersContactsContactUserIdGetRequest;

  try {
    const data = await api.getContactApiV1UsersContactsContactUserIdGet(body);
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
| **contactUserId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**ContactRead**](ContactRead.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getMeApiV1UsersMeGet

> UserRead getMeApiV1UsersMeGet()

Get Me

### Example

```ts
import {
  Configuration,
  UsersApi,
} from '@bianlat/api-client';
import type { GetMeApiV1UsersMeGetRequest } from '@bianlat/api-client';

async function example() {
  console.log("🚀 Testing @bianlat/api-client SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UsersApi(config);

  try {
    const data = await api.getMeApiV1UsersMeGet();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**UserRead**](UserRead.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listContactsApiV1UsersContactsGet

> CursorPageContactRead listContactsApiV1UsersContactsGet(q, cursor, size)

List Contacts

### Example

```ts
import {
  Configuration,
  UsersApi,
} from '@bianlat/api-client';
import type { ListContactsApiV1UsersContactsGetRequest } from '@bianlat/api-client';

async function example() {
  console.log("🚀 Testing @bianlat/api-client SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UsersApi(config);

  const body = {
    // string (optional)
    q: q_example,
    // string | Cursor for the next page (optional)
    cursor: cursor_example,
    // number | Page size (optional)
    size: 56,
  } satisfies ListContactsApiV1UsersContactsGetRequest;

  try {
    const data = await api.listContactsApiV1UsersContactsGet(body);
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
| **q** | `string` |  | [Optional] [Defaults to `undefined`] |
| **cursor** | `string` | Cursor for the next page | [Optional] [Defaults to `undefined`] |
| **size** | `number` | Page size | [Optional] [Defaults to `50`] |

### Return type

[**CursorPageContactRead**](CursorPageContactRead.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## removeContactApiV1UsersContactsContactUserIdDelete

> removeContactApiV1UsersContactsContactUserIdDelete(contactUserId)

Remove Contact

### Example

```ts
import {
  Configuration,
  UsersApi,
} from '@bianlat/api-client';
import type { RemoveContactApiV1UsersContactsContactUserIdDeleteRequest } from '@bianlat/api-client';

async function example() {
  console.log("🚀 Testing @bianlat/api-client SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UsersApi(config);

  const body = {
    // string
    contactUserId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies RemoveContactApiV1UsersContactsContactUserIdDeleteRequest;

  try {
    const data = await api.removeContactApiV1UsersContactsContactUserIdDelete(body);
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
| **contactUserId** | `string` |  | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateMeApiV1UsersMePatch

> UserRead updateMeApiV1UsersMePatch(userUpdate)

Update Me

### Example

```ts
import {
  Configuration,
  UsersApi,
} from '@bianlat/api-client';
import type { UpdateMeApiV1UsersMePatchRequest } from '@bianlat/api-client';

async function example() {
  console.log("🚀 Testing @bianlat/api-client SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UsersApi(config);

  const body = {
    // UserUpdate
    userUpdate: ...,
  } satisfies UpdateMeApiV1UsersMePatchRequest;

  try {
    const data = await api.updateMeApiV1UsersMePatch(body);
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
| **userUpdate** | [UserUpdate](UserUpdate.md) |  | |

### Return type

[**UserRead**](UserRead.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

