# CreateProjectRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **String** | Project name | 
**domain** | **String** | Website domain URL | 
**prompt** | Option<**String**> | Natural language prompt for crawling | [optional]
**search_query** | Option<**String**> | Search query for targeted crawling | [optional]
**sitemap_mode** | Option<**String**> | How to handle sitemaps | [optional][default to Include]
**include_subdomains** | Option<**bool**> | Whether to include subdomains | [optional][default to true]
**ignore_query_params** | Option<**bool**> | Whether to ignore URL query parameters | [optional][default to true]
**max_discovery_depth** | Option<**i32**> | Maximum crawl depth | [optional]
**exclude_paths** | Option<**Vec<String>**> | Paths to exclude from crawling | [optional]
**include_paths** | Option<**Vec<String>**> | Specific paths to include | [optional]
**crawl_entire_domain** | Option<**bool**> | Whether to crawl the entire domain | [optional][default to false]
**allow_external_links** | Option<**bool**> | Whether to allow external links | [optional][default to false]
**max_pages** | Option<**i32**> | Maximum number of pages to crawl | [optional][default to 100]
**crawl_delay** | Option<**i32**> | Delay between crawl requests (ms) | [optional]
**crawl_max_concurrency** | Option<**i32**> | Maximum concurrent crawl requests | [optional]
**only_main_content** | Option<**bool**> | Whether to extract only main content | [optional][default to true]
**custom_headers** | Option<**std::collections::HashMap<String, String>**> | Custom headers for crawling | [optional]
**wait_for** | Option<**i32**> | Wait time for page load (ms) | [optional][default to 0]
**block_ads** | Option<**bool**> | Whether to block ads | [optional][default to true]
**proxy_mode** | Option<**String**> | Proxy mode for crawling | [optional][default to Auto]
**use_reranking** | Option<**bool**> | Whether to use AI reranking | [optional][default to true]
**enable_change_tracking** | Option<**bool**> | Whether to enable change tracking | [optional][default to false]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


