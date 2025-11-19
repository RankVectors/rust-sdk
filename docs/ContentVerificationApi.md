# \ContentVerificationApi

All URIs are relative to *https://api.rankvectors.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_page_changes**](ContentVerificationApi.md#get_page_changes) | **GET** /api/projects/{projectId}/changes | Get page changes
[**verify_content**](ContentVerificationApi.md#verify_content) | **POST** /api/projects/{projectId}/verify-content | Verify page content



## get_page_changes

> models::GetPageChanges200Response get_page_changes(project_id, status, page_id, limit)
Get page changes

Get change history for pages in a project

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **String** | Unique identifier for the project | [required] |
**status** | Option<**String**> | Filter by change status |  |
**page_id** | Option<**String**> | Filter by page ID |  |
**limit** | Option<**i32**> | Results per page |  |[default to 50]

### Return type

[**models::GetPageChanges200Response**](getPageChanges_200_response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


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

