---
description: The high-level properties of a rule group. This, along with the <a>RuleGroup</a>, define the rule group. You can retrieve all objects for a rule group by calling <a>DescribeRuleGroup</a>.
layout: schema
name: RuleGroupResponse
properties_list:
- description: ''
  name: RuleGroupArn
  type: object
- description: ''
  name: RuleGroupName
  type: object
- description: ''
  name: RuleGroupId
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: Capacity
  type: object
- description: ''
  name: RuleGroupStatus
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: ConsumedCapacity
  type: object
- description: ''
  name: NumberOfAssociations
  type: object
- description: ''
  name: EncryptionConfiguration
  type: object
- description: ''
  name: SourceMetadata
  type: object
- description: ''
  name: SnsTopic
  type: object
- description: ''
  name: LastModifiedTime
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-rule-group-response-schema.json
slug: openapi-rule-group-response
source_filename: openapi-rule-group-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-rule-group-response-schema.json\",\n  \"title\": \"RuleGroupResponse\",\n  \"description\": \"The high-level properties of a rule group. This, along with the <a>RuleGroup</a>, define the rule group. You can retrieve all objects for a rule group by calling <a>DescribeRuleGroup</a>. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuleGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the rule group.</p> <note> <p>If this response is for a create request that had <code>DryRun</code> set to <code>TRUE</code>, then this ARN is a placeholder that isn't attached to a valid resource.</p> </note>\"\n        }\n      ]\n    },\n    \"RuleGroupName\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The descriptive name of the rule group. You can't change the name of a rule group after you create it.\"\n        }\n      ]\n    },\n    \"RuleGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The unique identifier for the rule group. \"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the rule group. \"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleGroupType\"\n        },\n        {\n          \"description\": \"Indicates whether the rule group is stateless or stateful. If the rule group is stateless,\
  \ it contains stateless rules. If it is stateful, it contains stateful rules. \"\n        }\n      ]\n    },\n    \"Capacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleCapacity\"\n        },\n        {\n          \"description\": \"<p>The maximum operating resources that this rule group can use. Rule group capacity is fixed at creation. When you update a rule group, you are limited to this capacity. When you reference a rule group from a firewall policy, Network Firewall reserves this capacity for the rule group. </p> <p>You can retrieve the capacity that would be required for a rule group before you create the rule group by calling <a>CreateRuleGroup</a> with <code>DryRun</code> set to <code>TRUE</code>. </p>\"\n        }\n      ]\n    },\n    \"RuleGroupStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceStatus\"\n        },\n        {\n          \"description\": \"Detailed information about the current\
  \ status of a rule group. \"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The key:value pairs to associate with the resource.\"\n        }\n      ]\n    },\n    \"ConsumedCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleCapacity\"\n        },\n        {\n          \"description\": \"The number of capacity units currently consumed by the rule group rules. \"\n        }\n      ]\n    },\n    \"NumberOfAssociations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NumberOfAssociations\"\n        },\n        {\n          \"description\": \"The number of firewall policies that use this rule group.\"\n        }\n      ]\n    },\n    \"EncryptionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionConfiguration\"\n        },\n       \
  \ {\n          \"description\": \"A complex type that contains the Amazon Web Services KMS encryption configuration settings for your rule group.\"\n        }\n      ]\n    },\n    \"SourceMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceMetadata\"\n        },\n        {\n          \"description\": \"A complex type that contains metadata about the rule group that your own rule group is copied from. You can use the metadata to track the version updates made to the originating rule group.\"\n        }\n      ]\n    },\n    \"SnsTopic\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon resource name (ARN) of the Amazon Simple Notification Service SNS topic that's used to record changes to the managed rule group. You can subscribe to the SNS topic to receive notifications when the managed rule group is modified, such as for new versions and\
  \ for version expiration. For more information, see the <a href=\\\"https://docs.aws.amazon.com/sns/latest/dg/welcome.html\\\">Amazon Simple Notification Service Developer Guide.</a>.\"\n        }\n      ]\n    },\n    \"LastModifiedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdateTime\"\n        },\n        {\n          \"description\": \"The last time that the rule group was changed.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RuleGroupArn\",\n    \"RuleGroupName\",\n    \"RuleGroupId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-rule-group-response-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: RuleGroupResponse
---
