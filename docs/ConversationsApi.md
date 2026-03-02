# ConversationsApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createConversationApiV1ConversationsPost**](ConversationsApi.md#createconversationapiv1conversationspost) | **POST** /api/v1/conversations | Create Conversation |
| [**deleteConversationApiV1ConversationsConversationIdDelete**](ConversationsApi.md#deleteconversationapiv1conversationsconversationiddelete) | **DELETE** /api/v1/conversations/{conversation_id} | Delete Conversation |
| [**getConversationApiV1ConversationsConversationIdGet**](ConversationsApi.md#getconversationapiv1conversationsconversationidget) | **GET** /api/v1/conversations/{conversation_id} | Get Conversation |
| [**listConversationsApiV1ConversationsGet**](ConversationsApi.md#listconversationsapiv1conversationsget) | **GET** /api/v1/conversations | List Conversations |



## createConversationApiV1ConversationsPost

> ConversationRead createConversationApiV1ConversationsPost(conversationCreate)

Create Conversation

### Example

```ts
import {
  Configuration,
  ConversationsApi,
} from '@bianlat/api-client';
import type { CreateConversationApiV1ConversationsPostRequest } from '@bianlat/api-client';

async function example() {
  console.log("🚀 Testing @bianlat/api-client SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ConversationsApi(config);

  const body = {
    // ConversationCreate
    conversationCreate: ...,
  } satisfies CreateConversationApiV1ConversationsPostRequest;

  try {
    const data = await api.createConversationApiV1ConversationsPost(body);
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
| **conversationCreate** | [ConversationCreate](ConversationCreate.md) |  | |

### Return type

[**ConversationRead**](ConversationRead.md)

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


## deleteConversationApiV1ConversationsConversationIdDelete

> deleteConversationApiV1ConversationsConversationIdDelete(conversationId)

Delete Conversation

### Example

```ts
import {
  Configuration,
  ConversationsApi,
} from '@bianlat/api-client';
import type { DeleteConversationApiV1ConversationsConversationIdDeleteRequest } from '@bianlat/api-client';

async function example() {
  console.log("🚀 Testing @bianlat/api-client SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ConversationsApi(config);

  const body = {
    // string
    conversationId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies DeleteConversationApiV1ConversationsConversationIdDeleteRequest;

  try {
    const data = await api.deleteConversationApiV1ConversationsConversationIdDelete(body);
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
| **conversationId** | `string` |  | [Defaults to `undefined`] |

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


## getConversationApiV1ConversationsConversationIdGet

> ConversationRead getConversationApiV1ConversationsConversationIdGet(conversationId)

Get Conversation

### Example

```ts
import {
  Configuration,
  ConversationsApi,
} from '@bianlat/api-client';
import type { GetConversationApiV1ConversationsConversationIdGetRequest } from '@bianlat/api-client';

async function example() {
  console.log("🚀 Testing @bianlat/api-client SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ConversationsApi(config);

  const body = {
    // string
    conversationId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies GetConversationApiV1ConversationsConversationIdGetRequest;

  try {
    const data = await api.getConversationApiV1ConversationsConversationIdGet(body);
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
| **conversationId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**ConversationRead**](ConversationRead.md)

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


## listConversationsApiV1ConversationsGet

> CursorPageConversationRead listConversationsApiV1ConversationsGet(cursor, size)

List Conversations

### Example

```ts
import {
  Configuration,
  ConversationsApi,
} from '@bianlat/api-client';
import type { ListConversationsApiV1ConversationsGetRequest } from '@bianlat/api-client';

async function example() {
  console.log("🚀 Testing @bianlat/api-client SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ConversationsApi(config);

  const body = {
    // string | Cursor for the next page (optional)
    cursor: cursor_example,
    // number | Page size (optional)
    size: 56,
  } satisfies ListConversationsApiV1ConversationsGetRequest;

  try {
    const data = await api.listConversationsApiV1ConversationsGet(body);
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
| **cursor** | `string` | Cursor for the next page | [Optional] [Defaults to `undefined`] |
| **size** | `number` | Page size | [Optional] [Defaults to `50`] |

### Return type

[**CursorPageConversationRead**](CursorPageConversationRead.md)

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

