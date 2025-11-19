# \AnalyticsApi

All URIs are relative to *https://api.rankvectors.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_project_analytics**](AnalyticsApi.md#get_project_analytics) | **GET** /api/projects/{projectId}/analytics | Get project analytics



## get_project_analytics

> models::ProjectAnalytics get_project_analytics(project_id, start_date, end_date)
Get project analytics

Get detailed analytics for a project

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **String** | Unique identifier for the project | [required] |
**start_date** | Option<**String**> | Start date for analytics |  |
**end_date** | Option<**String**> | End date for analytics |  |

### Return type

[**models::ProjectAnalytics**](ProjectAnalytics.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

