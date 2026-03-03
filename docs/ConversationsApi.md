# ConversationsApi

All URIs are relative to *http://localhost*

|Method | HTTP request | Description|
|------------- | ------------- | -------------|
|[**createConversationApiV1ConversationsPost**](#createconversationapiv1conversationspost) | **POST** /api/v1/conversations | Create Conversation|
|[**deleteConversationApiV1ConversationsConversationIdDelete**](#deleteconversationapiv1conversationsconversationiddelete) | **DELETE** /api/v1/conversations/{conversation_id} | Delete Conversation|
|[**getConversationApiV1ConversationsConversationIdGet**](#getconversationapiv1conversationsconversationidget) | **GET** /api/v1/conversations/{conversation_id} | Get Conversation|
|[**listConversationsApiV1ConversationsGet**](#listconversationsapiv1conversationsget) | **GET** /api/v1/conversations | List Conversations|

# **createConversationApiV1ConversationsPost**
> ConversationRead createConversationApiV1ConversationsPost(conversationCreate)


### Example

```typescript
import {
    ConversationsApi,
    Configuration,
    ConversationCreate
} from '@bianlat/api-client';

const configuration = new Configuration();
const apiInstance = new ConversationsApi(configuration);

let conversationCreate: ConversationCreate; //

const { status, data } = await apiInstance.createConversationApiV1ConversationsPost(
    conversationCreate
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **conversationCreate** | **ConversationCreate**|  | |


### Return type

**ConversationRead**

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

# **deleteConversationApiV1ConversationsConversationIdDelete**
> deleteConversationApiV1ConversationsConversationIdDelete()


### Example

```typescript
import {
    ConversationsApi,
    Configuration
} from '@bianlat/api-client';

const configuration = new Configuration();
const apiInstance = new ConversationsApi(configuration);

let conversationId: string; // (default to undefined)

const { status, data } = await apiInstance.deleteConversationApiV1ConversationsConversationIdDelete(
    conversationId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **conversationId** | [**string**] |  | defaults to undefined|


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

# **getConversationApiV1ConversationsConversationIdGet**
> ConversationRead getConversationApiV1ConversationsConversationIdGet()


### Example

```typescript
import {
    ConversationsApi,
    Configuration
} from '@bianlat/api-client';

const configuration = new Configuration();
const apiInstance = new ConversationsApi(configuration);

let conversationId: string; // (default to undefined)

const { status, data } = await apiInstance.getConversationApiV1ConversationsConversationIdGet(
    conversationId
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **conversationId** | [**string**] |  | defaults to undefined|


### Return type

**ConversationRead**

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

# **listConversationsApiV1ConversationsGet**
> CursorPageConversationRead listConversationsApiV1ConversationsGet()


### Example

```typescript
import {
    ConversationsApi,
    Configuration
} from '@bianlat/api-client';

const configuration = new Configuration();
const apiInstance = new ConversationsApi(configuration);

let cursor: string; //Cursor for the next page (optional) (default to undefined)
let size: number; //Page size (optional) (default to 50)

const { status, data } = await apiInstance.listConversationsApiV1ConversationsGet(
    cursor,
    size
);
```

### Parameters

|Name | Type | Description  | Notes|
|------------- | ------------- | ------------- | -------------|
| **cursor** | [**string**] | Cursor for the next page | (optional) defaults to undefined|
| **size** | [**number**] | Page size | (optional) defaults to 50|


### Return type

**CursorPageConversationRead**

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

