# \ImplementationsApi

All URIs are relative to *https://api.rankvectors.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_implementation**](ImplementationsApi.md#get_implementation) | **GET** /api/projects/{projectId}/implementations/{implementationId} | Get implementation details
[**implement_links**](ImplementationsApi.md#implement_links) | **POST** /api/projects/{projectId}/implementations | Implement link suggestions
[**list_implementations**](ImplementationsApi.md#list_implementations) | **GET** /api/projects/{projectId}/implementations | List implementations
[**rollback_implementation**](ImplementationsApi.md#rollback_implementation) | **POST** /api/projects/{projectId}/implementations/{implementationId}/rollback | Rollback implementation



## get_implementation

> models::GetImplementation200Response get_implementation(project_id, implementation_id)
Get implementation details

Get detailed information about a specific implementation

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **String** | Unique identifier for the project | [required] |
**implementation_id** | **String** | Unique identifier for the implementation | [required] |

### Return type

[**models::GetImplementation200Response**](getImplementation_200_response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## implement_links

> models::ImplementationResponse implement_links(project_id, implementation_request)
Implement link suggestions

Implement one or more link suggestions

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **String** | Unique identifier for the project | [required] |
**implementation_request** | [**ImplementationRequest**](ImplementationRequest.md) |  | [required] |

### Return type

[**models::ImplementationResponse**](ImplementationResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## list_implementations

> models::ListImplementations200Response list_implementations(project_id, status, platform, limit, offset)
List implementations

Get implementation history for a project

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **String** | Unique identifier for the project | [required] |
**status** | Option<**String**> | Filter by implementation status |  |
**platform** | Option<**String**> | Filter by platform |  |
**limit** | Option<**i32**> | Results per page |  |[default to 50]
**offset** | Option<**i32**> | Pagination offset |  |[default to 0]

### Return type

[**models::ListImplementations200Response**](listImplementations_200_response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## rollback_implementation

> models::RollbackImplementation200Response rollback_implementation(project_id, implementation_id, rollback_implementation_request)
Rollback implementation

Undo a link implementation and restore original content.  Rollback is universally available for all platforms: - WordPress (via custom/webhook) - Shopify (direct API) - Vercel (via custom/webhook) - Webflow (via custom/webhook) - Contentful (via custom/webhook) - Custom (via webhook)  The rollback process restores the original content that was stored during implementation. 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **String** | Unique identifier for the project | [required] |
**implementation_id** | **String** | Unique identifier for the implementation | [required] |
**rollback_implementation_request** | [**RollbackImplementationRequest**](RollbackImplementationRequest.md) |  | [required] |

### Return type

[**models::RollbackImplementation200Response**](rollbackImplementation_200_response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

