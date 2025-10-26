# Suggestion

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **String** | Unique suggestion identifier | 
**project_id** | **String** | Project identifier | 
**status** | **String** | Suggestion status | 
**relevance_score** | **f64** | AI-calculated relevance score (0-1) | 
**anchor_text** | **String** | Suggested anchor text | 
**context** | Option<**String**> | Context where the link should be placed | [optional]
**source_page** | [**models::PageInfo**](PageInfo.md) |  | 
**target_page** | [**models::PageInfo**](PageInfo.md) |  | 
**reasoning** | Option<**String**> | AI reasoning for the suggestion | [optional]
**created_at** | **String** | Suggestion creation timestamp | 
**updated_at** | Option<**String**> | Last update timestamp | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


