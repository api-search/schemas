---
description: <p>Describes a filter that returns a more specific list of recommendation export jobs. Use this filter with the <a>DescribeRecommendationExportJobs</a> action.</p> <p>You can use <code>EBSFilter</code> with the <a>GetEBSVolumeRecommendations</a> action, <code>LambdaFunctionRecommendationFilter</code> with the <a>GetLambdaFunctionRecommendations</a> action, and <code>Filter</code> with the <a>GetAutoScalingGroupRecommendations</a> and <a>GetEC2InstanceRecommendations</a> actions.</p>
layout: schema
name: JobFilter
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: values
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-job-filter-schema.json
slug: compute-optimizer-job-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-job-filter-schema.json\",\n  \"title\": \"JobFilter\",\n  \"description\": \"<p>Describes a filter that returns a more specific list of recommendation export jobs. Use this filter with the <a>DescribeRecommendationExportJobs</a> action.</p> <p>You can use <code>EBSFilter</code> with the <a>GetEBSVolumeRecommendations</a> action, <code>LambdaFunctionRecommendationFilter</code> with the <a>GetLambdaFunctionRecommendations</a> action, and <code>Filter</code> with the <a>GetAutoScalingGroupRecommendations</a> and <a>GetEC2InstanceRecommendations</a> actions.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobFilterName\"\n        },\n        {\n          \"description\": \"<p>The name\
  \ of the filter.</p> <p>Specify <code>ResourceType</code> to return export jobs of a specific resource type (for example, <code>Ec2Instance</code>).</p> <p>Specify <code>JobStatus</code> to return export jobs with a specific status (e.g, <code>Complete</code>).</p>\"\n        }\n      ]\n    },\n    \"values\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterValues\"\n        },\n        {\n          \"description\": \"<p>The value of the filter.</p> <p>The valid values for this parameter are as follows, depending on what you specify for the <code>name</code> parameter:</p> <ul> <li> <p>Specify <code>Ec2Instance</code> or <code>AutoScalingGroup</code> if you specify the <code>name</code> parameter as <code>ResourceType</code>. There is no filter for EBS volumes because volume recommendations cannot be exported at this time.</p> </li> <li> <p>Specify <code>Queued</code>, <code>InProgress</code>, <code>Complete</code>, or <code>Failed</code> if you specify\
  \ the <code>name</code> parameter as <code>JobStatus</code>.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-job-filter-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: JobFilter
---
