---
description: Describes an Lambda function recommendation.
layout: schema
name: LambdaFunctionRecommendation
properties_list:
- description: ''
  name: functionArn
  type: object
- description: ''
  name: functionVersion
  type: object
- description: ''
  name: accountId
  type: object
- description: ''
  name: currentMemorySize
  type: object
- description: ''
  name: numberOfInvocations
  type: object
- description: ''
  name: utilizationMetrics
  type: object
- description: ''
  name: lookbackPeriodInDays
  type: object
- description: ''
  name: lastRefreshTimestamp
  type: object
- description: ''
  name: finding
  type: object
- description: ''
  name: findingReasonCodes
  type: object
- description: ''
  name: memorySizeRecommendationOptions
  type: object
- description: ''
  name: currentPerformanceRisk
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-lambda-function-recommendation-schema.json
slug: compute-optimizer-lambda-function-recommendation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-lambda-function-recommendation-schema.json\",\n  \"title\": \"LambdaFunctionRecommendation\",\n  \"description\": \"Describes an Lambda function recommendation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"functionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FunctionArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the current function.\"\n        }\n      ]\n    },\n    \"functionVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FunctionVersion\"\n        },\n        {\n          \"description\": \"The version number of the current function.\"\n        }\n      ]\n    },\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID of the function.\"\n        }\n      ]\n    },\n    \"currentMemorySize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemorySize\"\n        },\n        {\n          \"description\": \"The amount of memory, in MB, that's allocated to the current function.\"\n        }\n      ]\n    },\n    \"numberOfInvocations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NumberOfInvocations\"\n        },\n        {\n          \"description\": \"The number of times your function code was applied during the look-back period.\"\n        }\n      ]\n    },\n    \"utilizationMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionUtilizationMetrics\"\n        },\n        {\n          \"description\": \"An array of objects that describe the utilization metrics of the function.\"\
  \n        }\n      ]\n    },\n    \"lookbackPeriodInDays\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LookBackPeriodInDays\"\n        },\n        {\n          \"description\": \"The number of days for which utilization metrics were analyzed for the function.\"\n        }\n      ]\n    },\n    \"lastRefreshTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastRefreshTimestamp\"\n        },\n        {\n          \"description\": \"The timestamp of when the function recommendation was last generated.\"\n        }\n      ]\n    },\n    \"finding\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionRecommendationFinding\"\n        },\n        {\n          \"description\": \"<p>The finding classification of the function.</p> <p>Findings for functions include:</p> <ul> <li> <p> <b> <code>Optimized</code> </b> \\u2014 The function is correctly provisioned to run your workload based\
  \ on its current configuration and its utilization history. This finding classification does not include finding reason codes.</p> </li> <li> <p> <b> <code>NotOptimized</code> </b> \\u2014 The function is performing at a higher level (over-provisioned) or at a lower level (under-provisioned) than required for your workload because its current configuration is not optimal. Over-provisioned resources might lead to unnecessary infrastructure cost, and under-provisioned resources might lead to poor application performance. This finding classification can include the <code>MemoryUnderprovisioned</code> and <code>MemoryUnderprovisioned</code> finding reason codes.</p> </li> <li> <p> <b> <code>Unavailable</code> </b> \\u2014 Compute Optimizer was unable to generate a recommendation for the function. This could be because the function has not accumulated sufficient metric data, or the function does not qualify for a recommendation. This finding classification can include the <code>InsufficientData</code>\
  \ and <code>Inconclusive</code> finding reason codes.</p> <note> <p>Functions with a finding of unavailable are not returned unless you specify the <code>filter</code> parameter with a value of <code>Unavailable</code> in your <code>GetLambdaFunctionRecommendations</code> request.</p> </note> </li> </ul>\"\n        }\n      ]\n    },\n    \"findingReasonCodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionRecommendationFindingReasonCodes\"\n        },\n        {\n          \"description\": \"<p>The reason for the finding classification of the function.</p> <note> <p>Functions that have a finding classification of <code>Optimized</code> don't have a finding reason code.</p> </note> <p>Finding reason codes for functions include:</p> <ul> <li> <p> <b> <code>MemoryOverprovisioned</code> </b> \\u2014 The function is over-provisioned when its memory configuration can be sized down while still meeting the performance requirements of your workload.\
  \ An over-provisioned function might lead to unnecessary infrastructure cost. This finding reason code is part of the <code>NotOptimized</code> finding classification.</p> </li> <li> <p> <b> <code>MemoryUnderprovisioned</code> </b> \\u2014 The function is under-provisioned when its memory configuration doesn't meet the performance requirements of the workload. An under-provisioned function might lead to poor application performance. This finding reason code is part of the <code>NotOptimized</code> finding classification.</p> </li> <li> <p> <b> <code>InsufficientData</code> </b> \\u2014 The function does not have sufficient metric data for Compute Optimizer to generate a recommendation. For more information, see the <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/requirements.html\\\">Supported resources and requirements</a> in the <i>Compute Optimizer User Guide</i>. This finding reason code is part of the <code>Unavailable</code> finding classification.</p> </li> <li>\
  \ <p> <b> <code>Inconclusive</code> </b> \\u2014 The function does not qualify for a recommendation because Compute Optimizer cannot generate a recommendation with a high degree of confidence. This finding reason code is part of the <code>Unavailable</code> finding classification.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"memorySizeRecommendationOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionMemoryRecommendationOptions\"\n        },\n        {\n          \"description\": \"An array of objects that describe the memory configuration recommendation options for the function.\"\n        }\n      ]\n    },\n    \"currentPerformanceRisk\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CurrentPerformanceRisk\"\n        },\n        {\n          \"description\": \"The risk of the current Lambda function not meeting the performance needs of its workloads. The higher the risk, the more likely the current\
  \ Lambda function requires more memory.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \" A list of tags assigned to your Lambda function recommendations. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-lambda-function-recommendation-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: LambdaFunctionRecommendation
---
