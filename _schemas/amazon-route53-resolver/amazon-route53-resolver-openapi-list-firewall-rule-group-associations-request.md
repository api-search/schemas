---
description: ListFirewallRuleGroupAssociationsRequest schema from openapi
layout: schema
name: ListFirewallRuleGroupAssociationsRequest
properties_list:
- description: ''
  name: FirewallRuleGroupId
  type: object
- description: ''
  name: VpcId
  type: object
- description: ''
  name: Priority
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Route 53 Resolver
provider_slug: amazon-route53-resolver
schema_file: json-schema/amazon-route53-resolver-openapi-list-firewall-rule-group-associations-request-schema.json
slug: amazon-route53-resolver-openapi-list-firewall-rule-group-associations-request
source_filename: amazon-route53-resolver-openapi-list-firewall-rule-group-associations-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-firewall-rule-group-associations-request-schema.json\",\n  \"title\": \"ListFirewallRuleGroupAssociationsRequest\",\n  \"description\": \"ListFirewallRuleGroupAssociationsRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallRuleGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The unique identifier of the firewall rule group that you want to retrieve the associations for. Leave this blank to retrieve associations for any rule group. \"\n        }\n      ]\n    },\n    \"VpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\":\
  \ \"The unique identifier of the VPC that you want to retrieve the associations for. Leave this blank to retrieve associations for any VPC. \"\n        }\n      ]\n    },\n    \"Priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Priority\"\n        },\n        {\n          \"description\": \"The setting that determines the processing order of the rule group among the rule groups that are associated with a single VPC. DNS Firewall filters VPC traffic starting from the rule group with the lowest numeric priority setting. \"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirewallRuleGroupAssociationStatus\"\n        },\n        {\n          \"description\": \"The association <code>Status</code> setting that you want DNS Firewall to filter on for the list. If you don't specify this, then DNS Firewall returns all associations, regardless of status.\"\n        }\n      ]\n    },\n\
  \    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"<p>The maximum number of objects that you want Resolver to return for this request. If more objects are available, in the response, Resolver provides a <code>NextToken</code> value that you can use in a subsequent call to get the next batch of objects.</p> <p>If you don't specify a value for <code>MaxResults</code>, Resolver returns up to 100 objects. </p>\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"<p>For the first call to this list request, omit this value.</p> <p>When you request a list of objects, Resolver returns at most the number of objects specified in <code>MaxResults</code>. If more objects are available for retrieval, Resolver returns a <code>NextToken</code> value in\
  \ the response. To retrieve the next batch of objects, use the token that was returned for the prior request in your next request.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-route53-resolver/refs/heads/main/json-schema/amazon-route53-resolver-openapi-list-firewall-rule-group-associations-request-schema.json
tags:
- AWS
- DNS
- Hybrid Cloud
- Networking
title: ListFirewallRuleGroupAssociationsRequest
---
