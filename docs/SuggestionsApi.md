# com.rankvectors\SuggestionsApi

All URIs are relative to *https://api.rankvectors.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**generate_suggestions**](SuggestionsApi.md#generate_suggestions) | **POST** /api/projects/{projectId}/suggestions | Generate link suggestions
[**get_suggestions**](SuggestionsApi.md#get_suggestions) | **GET** /api/projects/{projectId}/suggestions | Get link suggestions
[**update_suggestion**](SuggestionsApi.md#update_suggestion) | **PATCH** /api/projects/{projectId}/suggestions/{suggestionId} | Update suggestion status



## generate_suggestions

> models::GenerateSuggestions200Response generate_suggestions(project_id, generate_suggestions_request)
Generate link suggestions

Generate new AI-powered link suggestions for a project

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **String** | Unique identifier for the project | [required] |
**generate_suggestions_request** | Option<[**GenerateSuggestionsRequest**](GenerateSuggestionsRequest.md)> |  |  |

### Return type

[**models::GenerateSuggestions200Response**](generateSuggestions_200_response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_suggestions

> Vec<models::Suggestion> get_suggestions(project_id, status)
Get link suggestions

Get AI-generated link suggestions for a project

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **String** | Unique identifier for the project | [required] |
**status** | Option<**String**> | Filter suggestions by status |  |

### Return type

[**Vec<models::Suggestion>**](Suggestion.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_suggestion

> models::Suggestion update_suggestion(project_id, suggestion_id, update_suggestion_request)
Update suggestion status

Update the status of a link suggestion

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **String** | Unique identifier for the project | [required] |
**suggestion_id** | **String** | Unique identifier for the suggestion | [required] |
**update_suggestion_request** | [**UpdateSuggestionRequest**](UpdateSuggestionRequest.md) |  | [required] |

### Return type

[**models::Suggestion**](Suggestion.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

