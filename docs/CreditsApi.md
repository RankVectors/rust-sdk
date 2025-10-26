# com.rankvectors\CreditsApi

All URIs are relative to *https://api.rankvectors.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_credits**](CreditsApi.md#add_credits) | **POST** /api/projects/{projectId}/credits | Add credits
[**get_credits**](CreditsApi.md#get_credits) | **GET** /api/projects/{projectId}/credits | Get credit balance



## add_credits

> models::AddCredits200Response add_credits(project_id, add_credits_request)
Add credits

Add credits to a project (admin or payment webhook use)

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **String** | Unique identifier for the project | [required] |
**add_credits_request** | [**AddCreditsRequest**](AddCreditsRequest.md) |  | [required] |

### Return type

[**models::AddCredits200Response**](addCredits_200_response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_credits

> models::CreditBalance get_credits(project_id, include_history, start_date, end_date)
Get credit balance

Get credit balance and usage history for a project

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **String** | Unique identifier for the project | [required] |
**include_history** | Option<**bool**> | Include usage history |  |[default to false]
**start_date** | Option<**String**> | History start date (ISO 8601) |  |
**end_date** | Option<**String**> | History end date (ISO 8601) |  |

### Return type

[**models::CreditBalance**](CreditBalance.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

