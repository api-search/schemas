---
description: <p>Describes the scope of a recommendation preference.</p> <p>Recommendation preferences can be created at the organization level (for management accounts of an organization only), account level, and resource level. For more information, see <a href="https://docs.aws.amazon.com/compute-optimizer/latest/ug/enhanced-infrastructure-metrics.html">Activating enhanced infrastructure metrics</a> in the <i>Compute Optimizer User Guide</i>.</p> <note> <p>You cannot create recommendation preferences for Auto Scaling groups at the organization and account levels. You can create recommendation preferences for Auto Scaling groups only at the resource level by specifying a scope name of <code>ResourceArn</code> and a scope value of the Auto Scaling group Amazon Resource Name (ARN). This will configure the preference for all instances that are part of the specified Auto Scaling group. You also cannot create recommendation preferences at the resource level for instances that are part of an
  Auto Scaling group. You can create recommendation preferences at the resource level only for standalone instances.</p> </note>
layout: schema
name: Scope
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-scope-schema.json
slug: compute-optimizer-scope
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-scope-schema.json\",\n  \"title\": \"Scope\",\n  \"description\": \"<p>Describes the scope of a recommendation preference.</p> <p>Recommendation preferences can be created at the organization level (for management accounts of an organization only), account level, and resource level. For more information, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/enhanced-infrastructure-metrics.html\\\">Activating enhanced infrastructure metrics</a> in the <i>Compute Optimizer User Guide</i>.</p> <note> <p>You cannot create recommendation preferences for Auto Scaling groups at the organization and account levels. You can create recommendation preferences for Auto Scaling groups only at the resource level by specifying a scope name of <code>ResourceArn</code> and a\
  \ scope value of the Auto Scaling group Amazon Resource Name (ARN). This will configure the preference for all instances that are part of the specified Auto Scaling group. You also cannot create recommendation preferences at the resource level for instances that are part of an Auto Scaling group. You can create recommendation preferences at the resource level only for standalone instances.</p> </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScopeName\"\n        },\n        {\n          \"description\": \"<p>The name of the scope.</p> <p>The following scopes are possible:</p> <ul> <li> <p> <code>Organization</code> - Specifies that the recommendation preference applies at the organization level, for all member accounts of an organization.</p> </li> <li> <p> <code>AccountId</code> - Specifies that the recommendation preference applies at the account level, for all resources of a given resource\
  \ type in an account.</p> </li> <li> <p> <code>ResourceArn</code> - Specifies that the recommendation preference applies at the individual resource level.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScopeValue\"\n        },\n        {\n          \"description\": \"<p>The value of the scope.</p> <p>If you specified the <code>name</code> of the scope as:</p> <ul> <li> <p> <code>Organization</code> - The <code>value</code> must be <code>ALL_ACCOUNTS</code>.</p> </li> <li> <p> <code>AccountId</code> - The <code>value</code> must be a 12-digit Amazon Web Services account ID.</p> </li> <li> <p> <code>ResourceArn</code> - The <code>value</code> must be the Amazon Resource Name (ARN) of an EC2 instance or an Auto Scaling group.</p> </li> </ul> <p>Only EC2 instance and Auto Scaling group ARNs are currently supported.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-scope-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: Scope
---
