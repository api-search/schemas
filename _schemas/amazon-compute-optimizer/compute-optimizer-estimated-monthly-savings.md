---
description: <p>Describes the estimated monthly savings amount possible, based on On-Demand instance pricing, by adopting Compute Optimizer recommendations for a given resource.</p> <p>For more information, see <a href="https://docs.aws.amazon.com/compute-optimizer/latest/ug/view-ec2-recommendations.html#ec2-savings-calculation">Estimated monthly savings and savings opportunities</a> in the <i>Compute Optimizer User Guide</i>.</p>
layout: schema
name: EstimatedMonthlySavings
properties_list:
- description: ''
  name: currency
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-estimated-monthly-savings-schema.json
slug: compute-optimizer-estimated-monthly-savings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-estimated-monthly-savings-schema.json\",\n  \"title\": \"EstimatedMonthlySavings\",\n  \"description\": \"<p>Describes the estimated monthly savings amount possible, based on On-Demand instance pricing, by adopting Compute Optimizer recommendations for a given resource.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/view-ec2-recommendations.html#ec2-savings-calculation\\\">Estimated monthly savings and savings opportunities</a> in the <i>Compute Optimizer User Guide</i>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Currency\"\n        },\n        {\n          \"description\": \"The currency of the estimated monthly savings.\"\
  \n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Value\"\n        },\n        {\n          \"description\": \"The value of the estimated monthly savings.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-estimated-monthly-savings-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: EstimatedMonthlySavings
---
