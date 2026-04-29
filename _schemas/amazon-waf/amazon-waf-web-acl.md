---
description: Schema representing an AWS WAF Web ACL (Access Control List) resource.
layout: schema
name: AWS WAF Web ACL
properties_list:
- description: The name of the web ACL.
  name: Name
  type: string
- description: A unique identifier for the web ACL.
  name: Id
  type: string
- description: The Amazon Resource Name (ARN) of the web ACL.
  name: ARN
  type: string
- description: Specifies whether this is for CloudFront or for a regional application.
  name: Scope
  type: string
- description: The action to perform if none of the rules match.
  name: DefaultAction
  type: object
- description: The rules associated with the web ACL.
  name: Rules
  type: array
- description: Defines the CloudWatch metrics and sampling configuration.
  name: VisibilityConfig
  type: object
- description: The web ACL capacity units (WCUs) consumed by this web ACL.
  name: Capacity
  type: integer
- description: A token for optimistic locking.
  name: LockToken
  type: string
- description: Tags associated with the web ACL.
  name: Tags
  type: array
provider_name: Amazon WAF
provider_slug: amazon-waf
schema_file: json-schema/amazon-waf-web-acl-schema.json
slug: amazon-waf-web-acl
source_filename: amazon-waf-web-acl-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://wafv2.amazonaws.com/schemas/web-acl\",\n  \"title\": \"AWS WAF Web ACL\",\n  \"description\": \"Schema representing an AWS WAF Web ACL (Access Control List) resource.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"Name\",\n    \"Scope\",\n    \"DefaultAction\",\n    \"VisibilityConfig\"\n  ],\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the web ACL.\",\n      \"minLength\": 1,\n      \"maxLength\": 128,\n      \"pattern\": \"^[\\\\w+=:#@/\\\\-,.][\\\\w+=:#@/\\\\-,.\\\\s]+[\\\\w+=:#@/\\\\-,.]$\"\n    },\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the web ACL.\",\n      \"minLength\": 1,\n      \"maxLength\": 36,\n      \"pattern\": \"^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$\"\n    },\n    \"ARN\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The Amazon Resource Name (ARN) of the web ACL.\",\n      \"pattern\": \"^arn:aws:wafv2:.+:.+:.*/(web)?acl/.+\"\n    },\n    \"Scope\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies whether this is for CloudFront or for a regional application.\",\n      \"enum\": [\n        \"CLOUDFRONT\",\n        \"REGIONAL\"\n      ]\n    },\n    \"DefaultAction\": {\n      \"type\": \"object\",\n      \"description\": \"The action to perform if none of the rules match.\",\n      \"properties\": {\n        \"Allow\": {\n          \"type\": \"object\",\n          \"description\": \"Allow the request.\"\n        },\n        \"Block\": {\n          \"type\": \"object\",\n          \"description\": \"Block the request.\"\n        }\n      }\n    },\n    \"Rules\": {\n      \"type\": \"array\",\n      \"description\": \"The rules associated with the web ACL.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Rule\"\n      }\n    },\n    \"VisibilityConfig\": {\n      \"$ref\": \"\
  #/$defs/VisibilityConfig\",\n      \"description\": \"Defines the CloudWatch metrics and sampling configuration.\"\n    },\n    \"Capacity\": {\n      \"type\": \"integer\",\n      \"description\": \"The web ACL capacity units (WCUs) consumed by this web ACL.\"\n    },\n    \"LockToken\": {\n      \"type\": \"string\",\n      \"description\": \"A token for optimistic locking.\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags associated with the web ACL.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Rule\": {\n      \"type\": \"object\",\n      \"description\": \"A single rule in a web ACL.\",\n      \"required\": [\n        \"Name\",\n        \"Priority\",\n        \"VisibilityConfig\"\n      ],\n      \"properties\": {\n        \"Name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the rule.\"\n        },\n        \"Priority\": {\n          \"type\": \"integer\"\
  ,\n          \"description\": \"The processing priority of the rule.\"\n        },\n        \"Action\": {\n          \"type\": \"object\",\n          \"description\": \"The action to perform when the rule matches.\"\n        },\n        \"OverrideAction\": {\n          \"type\": \"object\",\n          \"description\": \"The override action to apply to rules in a rule group.\"\n        },\n        \"VisibilityConfig\": {\n          \"$ref\": \"#/$defs/VisibilityConfig\"\n        }\n      }\n    },\n    \"VisibilityConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Visibility configuration for CloudWatch metrics and request sampling.\",\n      \"required\": [\n        \"SampledRequestsEnabled\",\n        \"CloudWatchMetricsEnabled\",\n        \"MetricName\"\n      ],\n      \"properties\": {\n        \"SampledRequestsEnabled\": {\n          \"type\": \"boolean\"\n        },\n        \"CloudWatchMetricsEnabled\": {\n          \"type\": \"boolean\"\n        },\n        \"MetricName\"\
  : {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"Tag\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"Key\",\n        \"Value\"\n      ],\n      \"properties\": {\n        \"Key\": {\n          \"type\": \"string\",\n          \"minLength\": 1,\n          \"maxLength\": 128\n        },\n        \"Value\": {\n          \"type\": \"string\",\n          \"minLength\": 0,\n          \"maxLength\": 256\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-waf/refs/heads/main/json-schema/amazon-waf-web-acl-schema.json
tags:
- AWS
- Bot Management
- Ddos Protection
- Security
- WAF
- Web Application Firewall
title: AWS WAF Web ACL
---
