# com.rankvectors\WebhooksApi

All URIs are relative to *https://api.rankvectors.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_implementation_instructions**](WebhooksApi.md#get_implementation_instructions) | **GET** /api/webhook/implement-link | Get implementation instructions
[**report_implementation_status**](WebhooksApi.md#report_implementation_status) | **POST** /api/webhook/implement-link | Report implementation status



## get_implementation_instructions

> models::ImplementationInstructions get_implementation_instructions(suggestion_id)
Get implementation instructions

Get step-by-step instructions for implementing a link

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**suggestion_id** | **String** | ID of the suggestion to implement | [required] |

### Return type

[**models::ImplementationInstructions**](ImplementationInstructions.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## report_implementation_status

> models::ReportImplementationStatus200Response report_implementation_status(report_implementation_status_request)
Report implementation status

Report the status of a link implementation

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**report_implementation_status_request** | [**ReportImplementationStatusRequest**](ReportImplementationStatusRequest.md) |  | [required] |

### Return type

[**models::ReportImplementationStatus200Response**](reportImplementationStatus_200_response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

