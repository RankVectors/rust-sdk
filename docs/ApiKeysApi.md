# \ApiKeysApi

All URIs are relative to *https://api.rankvectors.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_api_key**](ApiKeysApi.md#create_api_key) | **POST** /api/api-keys | Create API key
[**delete_api_key**](ApiKeysApi.md#delete_api_key) | **DELETE** /api/api-keys/{id} | Delete API key
[**list_api_keys**](ApiKeysApi.md#list_api_keys) | **GET** /api/api-keys | List API keys
[**update_api_key**](ApiKeysApi.md#update_api_key) | **PATCH** /api/api-keys/{id} | Update API key



## create_api_key

> models::ApiKeyResponse create_api_key(create_api_key_request)
Create API key

Create a new API key for the authenticated user

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_api_key_request** | [**CreateApiKeyRequest**](CreateApiKeyRequest.md) |  | [required] |

### Return type

[**models::ApiKeyResponse**](ApiKeyResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_api_key

> models::DeleteSuggestion200Response delete_api_key(id)
Delete API key

Delete an API key

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | API key ID | [required] |

### Return type

[**models::DeleteSuggestion200Response**](deleteSuggestion_200_response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## list_api_keys

> Vec<models::ApiKey> list_api_keys()
List API keys

Get all API keys for the authenticated user

### Parameters

This endpoint does not need any parameter.

### Return type

[**Vec<models::ApiKey>**](ApiKey.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_api_key

> models::ApiKey update_api_key(id, update_api_key_request)
Update API key

Update an API key (activate/deactivate or change name)

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**id** | **String** | API key ID | [required] |
**update_api_key_request** | [**UpdateApiKeyRequest**](UpdateApiKeyRequest.md) |  | [required] |

### Return type

[**models::ApiKey**](ApiKey.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

