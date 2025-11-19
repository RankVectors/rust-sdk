# \ProjectsApi

All URIs are relative to *https://api.rankvectors.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_project**](ProjectsApi.md#create_project) | **POST** /api/projects | Create a new project
[**delete_project**](ProjectsApi.md#delete_project) | **DELETE** /api/projects/{projectId} | Delete a project
[**get_project**](ProjectsApi.md#get_project) | **GET** /api/projects/{projectId} | Get project details
[**list_projects**](ProjectsApi.md#list_projects) | **GET** /api/projects | List all projects
[**sync_project**](ProjectsApi.md#sync_project) | **POST** /api/projects/{projectId}/sync | Sync project



## create_project

> models::Project create_project(create_project_request)
Create a new project

Create a new project for internal linking optimization

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_project_request** | [**CreateProjectRequest**](CreateProjectRequest.md) |  | [required] |

### Return type

[**models::Project**](Project.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_project

> models::DeleteProject200Response delete_project(project_id)
Delete a project

Delete a project and all associated data

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **String** | Unique identifier for the project | [required] |

### Return type

[**models::DeleteProject200Response**](deleteProject_200_response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_project

> models::Project get_project(project_id)
Get project details

Get detailed information about a specific project

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **String** | Unique identifier for the project | [required] |

### Return type

[**models::Project**](Project.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## list_projects

> Vec<models::Project> list_projects()
List all projects

Get a list of all projects for the authenticated user

### Parameters

This endpoint does not need any parameter.

### Return type

[**Vec<models::Project>**](Project.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## sync_project

> models::SyncProject200Response sync_project(project_id, sync_project_request)
Sync project

Trigger a full sync of project content (used by WordPress and other integrations)

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**project_id** | **String** | Unique identifier for the project | [required] |
**sync_project_request** | Option<[**SyncProjectRequest**](SyncProjectRequest.md)> |  |  |

### Return type

[**models::SyncProject200Response**](syncProject_200_response.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

