# UsersApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**addContactApiV1UsersContactsPost**](#addcontactapiv1userscontactspost) | **POST** /api/v1/users/contacts | Add Contact|
|[**getContactApiV1UsersContactsContactUserIdGet**](#getcontactapiv1userscontactscontactuseridget) | **GET** /api/v1/users/contacts/{contact_user_id} | Get Contact|
|[**getMeApiV1UsersMeGet**](#getmeapiv1usersmeget) | **GET** /api/v1/users/me | Get Me|
|[**listContactsApiV1UsersContactsGet**](#listcontactsapiv1userscontactsget) | **GET** /api/v1/users/contacts | List Contacts|
|[**removeContactApiV1UsersContactsContactIdDelete**](#removecontactapiv1userscontactscontactiddelete) | **DELETE** /api/v1/users/contacts/{contact_id} | Remove Contact|
|[**updateContactApiV1UsersContactsContactIdPatch**](#updatecontactapiv1userscontactscontactidpatch) | **PATCH** /api/v1/users/contacts/{contact_id} | Update Contact|
|[**updateMeApiV1UsersMePatch**](#updatemeapiv1usersmepatch) | **PATCH** /api/v1/users/me | Update Me|

# **addContactApiV1UsersContactsPost**
> ContactAddResult addContactApiV1UsersContactsPost(contactCreate)


### Example

```typescript
import {
    UsersApi,
    Configuration,
    ContactCreate
} from '@bianlat/api-client';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let contactCreate: ContactCreate; //

const { status, data } = await apiInstance.addContactApiV1UsersContactsPost(
    contactCreate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **contactCreate** | **ContactCreate**|  | |


### Return type

**ContactAddResult**

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

# **getContactApiV1UsersContactsContactUserIdGet**
> ContactRead getContactApiV1UsersContactsContactUserIdGet()


### Example

```typescript
import {
    UsersApi,
    Configuration
} from '@bianlat/api-client';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let contactUserId: string; // (default to undefined)

const { status, data } = await apiInstance.getContactApiV1UsersContactsContactUserIdGet(
    contactUserId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **contactUserId** | [**string**] |  | defaults to undefined|


### Return type

**ContactRead**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **getMeApiV1UsersMeGet**
> UserRead getMeApiV1UsersMeGet()


### Example

```typescript
import {
    UsersApi,
    Configuration
} from '@bianlat/api-client';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

const { status, data } = await apiInstance.getMeApiV1UsersMeGet();
```

### Parameters
This endpoint does not have any parameters.


### Return type

**UserRead**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **listContactsApiV1UsersContactsGet**
> CursorPageContactRead listContactsApiV1UsersContactsGet()


### Example

```typescript
import {
    UsersApi,
    Configuration
} from '@bianlat/api-client';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let q: string; // (optional) (default to undefined)
let status: 'pending_registration'; // (optional) (default to undefined)
let cursor: string; //Cursor for the next page (optional) (default to undefined)
let size: number; //Page size (optional) (default to 50)

const { status, data } = await apiInstance.listContactsApiV1UsersContactsGet(
    q,
    status,
    cursor,
    size
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **q** | [**string**] |  | (optional) defaults to undefined|
| **status** | [**&#39;pending_registration&#39;**]**Array<&#39;pending_registration&#39; &#124; &#39;11184809&#39;>** |  | (optional) defaults to undefined|
| **cursor** | [**string**] | Cursor for the next page | (optional) defaults to undefined|
| **size** | [**number**] | Page size | (optional) defaults to 50|


### Return type

**CursorPageContactRead**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **removeContactApiV1UsersContactsContactIdDelete**
> removeContactApiV1UsersContactsContactIdDelete()


### Example

```typescript
import {
    UsersApi,
    Configuration
} from '@bianlat/api-client';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let contactId: string; // (default to undefined)

const { status, data } = await apiInstance.removeContactApiV1UsersContactsContactIdDelete(
    contactId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **contactId** | [**string**] |  | defaults to undefined|


### Return type

void (empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**204** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateContactApiV1UsersContactsContactIdPatch**
> ContactRead updateContactApiV1UsersContactsContactIdPatch(contactUpdate)


### Example

```typescript
import {
    UsersApi,
    Configuration,
    ContactUpdate
} from '@bianlat/api-client';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let contactId: string; // (default to undefined)
let contactUpdate: ContactUpdate; //

const { status, data } = await apiInstance.updateContactApiV1UsersContactsContactIdPatch(
    contactId,
    contactUpdate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **contactUpdate** | **ContactUpdate**|  | |
| **contactId** | [**string**] |  | defaults to undefined|


### Return type

**ContactRead**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **updateMeApiV1UsersMePatch**
> UserRead updateMeApiV1UsersMePatch(userUpdate)


### Example

```typescript
import {
    UsersApi,
    Configuration,
    UserUpdate
} from '@bianlat/api-client';

const configuration = new Configuration();
const apiInstance = new UsersApi(configuration);

let userUpdate: UserUpdate; //

const { status, data } = await apiInstance.updateMeApiV1UsersMePatch(
    userUpdate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **userUpdate** | **UserUpdate**|  | |


### Return type

**UserRead**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
|**200** | Successful Response |  -  |
|**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

