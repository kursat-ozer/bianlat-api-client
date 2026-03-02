# @bianlat/api-client@0.0.1

A TypeScript SDK client for the localhost API.

## Usage

First, install the SDK from npm.

```bash
npm install @bianlat/api-client --save
```

Next, try it out.


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


## Documentation

### API Endpoints

All URIs are relative to *http://localhost*

| Class | Method | HTTP request | Description
| ----- | ------ | ------------ | -------------
*AuthApi* | [**loginApiV1AuthLoginPost**](docs/AuthApi.md#loginapiv1authloginpost) | **POST** /api/v1/auth/login | Login
*AuthApi* | [**logoutApiV1AuthLogoutPost**](docs/AuthApi.md#logoutapiv1authlogoutpost) | **POST** /api/v1/auth/logout | Logout
*AuthApi* | [**refreshApiV1AuthRefreshPost**](docs/AuthApi.md#refreshapiv1authrefreshpost) | **POST** /api/v1/auth/refresh | Refresh
*AuthApi* | [**verifyApiV1AuthVerifyPost**](docs/AuthApi.md#verifyapiv1authverifypost) | **POST** /api/v1/auth/verify | Verify
*ConversationsApi* | [**createConversationApiV1ConversationsPost**](docs/ConversationsApi.md#createconversationapiv1conversationspost) | **POST** /api/v1/conversations | Create Conversation
*ConversationsApi* | [**deleteConversationApiV1ConversationsConversationIdDelete**](docs/ConversationsApi.md#deleteconversationapiv1conversationsconversationiddelete) | **DELETE** /api/v1/conversations/{conversation_id} | Delete Conversation
*ConversationsApi* | [**getConversationApiV1ConversationsConversationIdGet**](docs/ConversationsApi.md#getconversationapiv1conversationsconversationidget) | **GET** /api/v1/conversations/{conversation_id} | Get Conversation
*ConversationsApi* | [**listConversationsApiV1ConversationsGet**](docs/ConversationsApi.md#listconversationsapiv1conversationsget) | **GET** /api/v1/conversations | List Conversations
*HealthApi* | [**healthHealthGet**](docs/HealthApi.md#healthhealthget) | **GET** /health | Health
*MessagesApi* | [**getMessagesApiV1ConversationsConversationIdMessagesGet**](docs/MessagesApi.md#getmessagesapiv1conversationsconversationidmessagesget) | **GET** /api/v1/conversations/{conversation_id}/messages | Get Messages
*MessagesApi* | [**markAsReadApiV1MessagesMessageIdReadPatch**](docs/MessagesApi.md#markasreadapiv1messagesmessageidreadpatch) | **PATCH** /api/v1/messages/{message_id}/read | Mark As Read
*MessagesApi* | [**sendMessageApiV1ConversationsConversationIdMessagesPost**](docs/MessagesApi.md#sendmessageapiv1conversationsconversationidmessagespost) | **POST** /api/v1/conversations/{conversation_id}/messages | Send Message
*UsersApi* | [**addContactApiV1UsersContactsPost**](docs/UsersApi.md#addcontactapiv1userscontactspost) | **POST** /api/v1/users/contacts | Add Contact
*UsersApi* | [**getContactApiV1UsersContactsContactUserIdGet**](docs/UsersApi.md#getcontactapiv1userscontactscontactuseridget) | **GET** /api/v1/users/contacts/{contact_user_id} | Get Contact
*UsersApi* | [**getMeApiV1UsersMeGet**](docs/UsersApi.md#getmeapiv1usersmeget) | **GET** /api/v1/users/me | Get Me
*UsersApi* | [**listContactsApiV1UsersContactsGet**](docs/UsersApi.md#listcontactsapiv1userscontactsget) | **GET** /api/v1/users/contacts | List Contacts
*UsersApi* | [**removeContactApiV1UsersContactsContactUserIdDelete**](docs/UsersApi.md#removecontactapiv1userscontactscontactuseriddelete) | **DELETE** /api/v1/users/contacts/{contact_user_id} | Remove Contact
*UsersApi* | [**updateMeApiV1UsersMePatch**](docs/UsersApi.md#updatemeapiv1usersmepatch) | **PATCH** /api/v1/users/me | Update Me


### Models

- [ContactCreate](docs/ContactCreate.md)
- [ContactRead](docs/ContactRead.md)
- [ConversationCreate](docs/ConversationCreate.md)
- [ConversationRead](docs/ConversationRead.md)
- [ConversationType](docs/ConversationType.md)
- [CursorPageContactRead](docs/CursorPageContactRead.md)
- [CursorPageConversationRead](docs/CursorPageConversationRead.md)
- [HTTPValidationError](docs/HTTPValidationError.md)
- [HealthResponse](docs/HealthResponse.md)
- [LastMessageRead](docs/LastMessageRead.md)
- [LocationInner](docs/LocationInner.md)
- [LoginRequest](docs/LoginRequest.md)
- [MessageRead](docs/MessageRead.md)
- [MessageStatus](docs/MessageStatus.md)
- [MessageType](docs/MessageType.md)
- [PaginatedMessages](docs/PaginatedMessages.md)
- [ParticipantRead](docs/ParticipantRead.md)
- [ParticipantRole](docs/ParticipantRole.md)
- [RefreshRequest](docs/RefreshRequest.md)
- [SendMessageRequest](docs/SendMessageRequest.md)
- [TokenResponse](docs/TokenResponse.md)
- [UserRead](docs/UserRead.md)
- [UserUpdate](docs/UserUpdate.md)
- [ValidationError](docs/ValidationError.md)
- [VerifyRequest](docs/VerifyRequest.md)

### Authorization


Authentication schemes defined for the API:
<a id="HTTPBearer"></a>
#### HTTPBearer


- **Type**: HTTP Bearer Token authentication

## About

This TypeScript SDK client supports the [Fetch API](https://fetch.spec.whatwg.org/)
and is automatically generated by the
[OpenAPI Generator](https://openapi-generator.tech) project:

- API version: `0.0.2`
- Package version: `0.0.1`
- Generator version: `7.20.0`
- Build package: `org.openapitools.codegen.languages.TypeScriptFetchClientCodegen`

The generated npm module supports the following:

- Environments
  * Node.js
  * Webpack
  * Browserify
- Language levels
  * ES5 - you must have a Promises/A+ library installed
  * ES6
- Module systems
  * CommonJS
  * ES6 module system


## Development

### Building

To build the TypeScript source code, you need to have Node.js and npm installed.
After cloning the repository, navigate to the project directory and run:

```bash
npm install
npm run build
```

### Publishing

Once you've built the package, you can publish it to npm:

```bash
npm publish
```

## License

[]()
