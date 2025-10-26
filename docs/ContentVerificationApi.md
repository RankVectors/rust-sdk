# com.rankvectors\ContentVerificationApi

All URIs are relative to *https://api.rankvectors.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**verify_content**](ContentVerificationApi.md#verify_content) | **POST** /api/projects/{projectId}/verify-content | Verify page content



## verify_content

> models::VerifyContent200Response verify_content(project_id, verify_content_request)
Verify page content

Check if page content has changed since last crawl

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **String** | Unique identifier for the project | [required] |
**verify_content_request** | [**VerifyContentRequest**](VerifyContentRequest.md) |  | [required] |

### Return type

[**models::VerifyContent200Response**](verifyContent_200_response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

