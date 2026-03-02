# HealthApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**healthHealthGet**](HealthApi.md#healthhealthget) | **GET** /health | Health |



## healthHealthGet

> any healthHealthGet()

Health

### Example

```ts
import {
  Configuration,
  HealthApi,
} from '@bianlat/api-client';
import type { HealthHealthGetRequest } from '@bianlat/api-client';

async function example() {
  console.log("🚀 Testing @bianlat/api-client SDK...");
  const api = new HealthApi();

  try {
    const data = await api.healthHealthGet();
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

**any**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

