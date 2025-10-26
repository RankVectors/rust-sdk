# com.rankvectors\CrawlingApi

All URIs are relative to *https://api.rankvectors.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_crawl_history**](CrawlingApi.md#get_crawl_history) | **GET** /api/projects/{projectId}/crawl | Get crawl history
[**start_crawl**](CrawlingApi.md#start_crawl) | **POST** /api/projects/{projectId}/crawl | Start website crawl



## get_crawl_history

> Vec<models::Crawl> get_crawl_history(project_id)
Get crawl history

Get the crawl history for a project

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **String** | Unique identifier for the project | [required] |

### Return type

[**Vec<models::Crawl>**](Crawl.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## start_crawl

> models::Crawl start_crawl(project_id, start_crawl_request)
Start website crawl

Start crawling a website to analyze content for link opportunities

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **String** | Unique identifier for the project | [required] |
**start_crawl_request** | Option<[**StartCrawlRequest**](StartCrawlRequest.md)> |  |  |

### Return type

[**models::Crawl**](Crawl.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

