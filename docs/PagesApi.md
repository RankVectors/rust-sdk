# \PagesApi

All URIs are relative to *https://api.rankvectors.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**batch_sync_pages**](PagesApi.md#batch_sync_pages) | **POST** /api/projects/{projectId}/pages/batch | Batch sync pages
[**list_pages**](PagesApi.md#list_pages) | **GET** /api/projects/{projectId}/pages | List pages



## batch_sync_pages

> models::BatchSyncPages200Response batch_sync_pages(project_id, batch_sync_pages_request)
Batch sync pages

Sync multiple pages to a project (used by WordPress and other integrations)

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **String** | Unique identifier for the project | [required] |
**batch_sync_pages_request** | [**BatchSyncPagesRequest**](BatchSyncPagesRequest.md) |  | [required] |

### Return type

[**models::BatchSyncPages200Response**](batchSyncPages_200_response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## list_pages

> models::ListPages200Response list_pages(project_id, limit, offset)
List pages

Get a list of pages for a project

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **String** | Unique identifier for the project | [required] |
**limit** | Option<**i32**> | Results per page |  |[default to 50]
**offset** | Option<**i32**> | Pagination offset |  |[default to 0]

### Return type

[**models::ListPages200Response**](listPages_200_response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

