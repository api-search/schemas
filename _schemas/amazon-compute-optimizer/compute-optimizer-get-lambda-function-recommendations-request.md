---
description: GetLambdaFunctionRecommendationsRequest schema
layout: schema
name: GetLambdaFunctionRecommendationsRequest
properties_list:
- description: ''
  name: functionArns
  type: object
- description: ''
  name: accountIds
  type: object
- description: ''
  name: filters
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-get-lambda-function-recommendations-request-schema.json
slug: compute-optimizer-get-lambda-function-recommendations-request
source_filename: compute-optimizer-get-lambda-function-recommendations-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-lambda-function-recommendations-request-schema.json\",\n  \"title\": \"GetLambdaFunctionRecommendationsRequest\",\n  \"description\": \"GetLambdaFunctionRecommendationsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"functionArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FunctionArns\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the functions for which to return recommendations.</p> <p>You can specify a qualified or unqualified ARN. If you specify an unqualified ARN without a function version suffix, Compute Optimizer will return recommendations for the latest (<code>$LATEST</code>) version of the function. If you specify a qualified ARN with a version suffix, Compute\
  \ Optimizer will return recommendations for the specified function version. For more information about using function versions, see <a href=\\\"https://docs.aws.amazon.com/lambda/latest/dg/configuration-versions.html#versioning-versions-using\\\">Using versions</a> in the <i>Lambda Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"accountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountIds\"\n        },\n        {\n          \"description\": \"<p>The ID of the Amazon Web Services account for which to return function recommendations.</p> <p>If your account is the management account of an organization, use this parameter to specify the member account for which you want to return function recommendations.</p> <p>Only one account ID can be specified per request.</p>\"\n        }\n      ]\n    },\n    \"filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionRecommendationFilters\"\n        },\n\
  \        {\n          \"description\": \"An array of objects to specify a filter that returns a more specific list of function recommendations.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to advance to the next page of function recommendations.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"<p>The maximum number of function recommendations to return with a single request.</p> <p>To retrieve the remaining results, make another request with the returned <code>nextToken</code> value.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-lambda-function-recommendations-request-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: GetLambdaFunctionRecommendationsRequest
---
