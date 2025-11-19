# Implementation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **String** | Unique implementation identifier | 
**status** | **String** | Implementation status | 
**platform** | **String** | Platform used | 
**implementation_method** | Option<**String**> | Implementation method | [optional]
**credits_used** | Option<**f64**> | Credits consumed | [optional]
**created_at** | **String** | Implementation start timestamp | 
**completed_at** | Option<**String**> | Implementation completion timestamp | [optional]
**metadata** | Option<[**std::collections::HashMap<String, serde_json::Value>**](serde_json::Value.md)> | Platform-specific metadata | [optional]
**suggestion** | [**models::Suggestion**](Suggestion.md) |  | 
**rollbacks** | Option<[**Vec<models::Rollback>**](Rollback.md)> | Rollback history | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


