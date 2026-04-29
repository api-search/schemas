---
description: UpdateRuleGroupRequest schema from Amazon Network Firewall
layout: schema
name: UpdateRuleGroupRequest
properties_list:
- description: ''
  name: UpdateToken
  type: object
- description: ''
  name: RuleGroupArn
  type: object
- description: ''
  name: RuleGroupName
  type: object
- description: ''
  name: RuleGroup
  type: object
- description: ''
  name: Rules
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: DryRun
  type: object
- description: ''
  name: EncryptionConfiguration
  type: object
- description: ''
  name: SourceMetadata
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-update-rule-group-request-schema.json
slug: openapi-update-rule-group-request
source_filename: openapi-update-rule-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-update-rule-group-request-schema.json\",\n  \"title\": \"UpdateRuleGroupRequest\",\n  \"description\": \"UpdateRuleGroupRequest schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UpdateToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateToken\"\n        },\n        {\n          \"description\": \"<p>A token used for optimistic locking. Network Firewall returns a token to your requests that access the rule group. The token marks the state of the rule group resource at the time of the request. </p> <p>To make changes to the rule group, you provide the token in your request. Network Firewall uses the token to ensure that the rule group hasn't changed since you last retrieved it. If it has changed, the operation\
  \ fails with an <code>InvalidTokenException</code>. If this happens, retrieve the rule group again to get a current copy of it with a current token. Reapply your changes as needed, then try the operation again using the new token. </p>\"\n        }\n      ]\n    },\n    \"RuleGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the rule group.</p> <p>You must specify the ARN or the name, and you can specify both. </p>\"\n        }\n      ]\n    },\n    \"RuleGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"<p>The descriptive name of the rule group. You can't change the name of a rule group after you create it.</p> <p>You must specify the ARN or the name, and you can specify both. </p>\"\n        }\n      ]\n    },\n    \"RuleGroup\": {\n   \
  \   \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleGroup\"\n        },\n        {\n          \"description\": \"<p>An object that defines the rule group rules. </p> <note> <p>You must provide either this rule group setting or a <code>Rules</code> setting, but not both. </p> </note>\"\n        }\n      ]\n    },\n    \"Rules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RulesString\"\n        },\n        {\n          \"description\": \"<p>A string containing stateful rule group rules specifications in Suricata flat format, with one rule per line. Use this to import your existing Suricata compatible rule groups. </p> <note> <p>You must provide either this rules setting or a populated <code>RuleGroup</code> setting, but not both. </p> </note> <p>You can provide your rule group specification in Suricata flat format through this setting when you create or update your rule group. The call response returns a <a>RuleGroup</a> object that\
  \ Network Firewall has populated from your string. </p>\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleGroupType\"\n        },\n        {\n          \"description\": \"<p>Indicates whether the rule group is stateless or stateful. If the rule group is stateless, it contains stateless rules. If it is stateful, it contains stateful rules. </p> <note> <p>This setting is required for requests that do not include the <code>RuleGroupARN</code>.</p> </note>\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description of the rule group. \"\n        }\n      ]\n    },\n    \"DryRun\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>Indicates whether you want Network Firewall to\
  \ just check the validity of the request, rather than run the request. </p> <p>If set to <code>TRUE</code>, Network Firewall checks whether the request can run successfully, but doesn't actually make the requested changes. The call returns the value that the request would return if you ran it with dry run set to <code>FALSE</code>, but doesn't make additions or changes to your resources. This option allows you to make sure that you have the required permissions to run the request and that your request parameters are valid. </p> <p>If set to <code>FALSE</code>, Network Firewall makes the requested changes to your resources. </p>\"\n        }\n      ]\n    },\n    \"EncryptionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionConfiguration\"\n        },\n        {\n          \"description\": \"A complex type that contains settings for encryption of your rule group resources.\"\n        }\n      ]\n    },\n    \"SourceMetadata\": {\n  \
  \    \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceMetadata\"\n        },\n        {\n          \"description\": \"A complex type that contains metadata about the rule group that your own rule group is copied from. You can use the metadata to keep track of updates made to the originating rule group.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UpdateToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-update-rule-group-request-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: UpdateRuleGroupRequest
---
