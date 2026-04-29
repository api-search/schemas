---
description: A list that contains detailed configurations of a specified resource.
layout: schema
name: ConfigurationItem
properties_list:
- description: ''
  name: version
  type: object
- description: ''
  name: accountId
  type: object
- description: ''
  name: configurationItemCaptureTime
  type: object
- description: ''
  name: configurationItemStatus
  type: object
- description: ''
  name: configurationStateId
  type: object
- description: ''
  name: configurationItemMD5Hash
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: resourceType
  type: object
- description: ''
  name: resourceId
  type: object
- description: ''
  name: resourceName
  type: object
- description: ''
  name: awsRegion
  type: object
- description: ''
  name: availabilityZone
  type: object
- description: ''
  name: resourceCreationTime
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: relatedEvents
  type: object
- description: ''
  name: relationships
  type: object
- description: ''
  name: configuration
  type: object
- description: ''
  name: supplementaryConfiguration
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-configuration-item-schema.json
slug: config-configuration-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-configuration-item-schema.json\",\n  \"title\": \"ConfigurationItem\",\n  \"description\": \"A list that contains detailed configurations of a specified resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"The version number of the resource configuration.\"\n        }\n      ]\n    },\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The 12-digit Amazon Web Services account ID associated with the resource.\"\n        }\n      ]\n    },\n    \"configurationItemCaptureTime\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/ConfigurationItemCaptureTime\"\n        },\n        {\n          \"description\": \"The time when the configuration recording was initiated.\"\n        }\n      ]\n    },\n    \"configurationItemStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationItemStatus\"\n        },\n        {\n          \"description\": \"<p>The configuration item status. The valid values are:</p> <ul> <li> <p>OK \\u2013 The resource configuration has been updated</p> </li> <li> <p>ResourceDiscovered \\u2013 The resource was newly discovered</p> </li> <li> <p>ResourceNotRecorded \\u2013 The resource was discovered but its configuration was not recorded since the recorder excludes the recording of resources of this type</p> </li> <li> <p>ResourceDeleted \\u2013 The resource was deleted</p> </li> <li> <p>ResourceDeletedNotRecorded \\u2013 The resource was deleted but its configuration was not recorded since the recorder excludes the recording\
  \ of resources of this type</p> </li> </ul> <note> <p>The CIs do not incur any cost.</p> </note>\"\n        }\n      ]\n    },\n    \"configurationStateId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationStateId\"\n        },\n        {\n          \"description\": \"An identifier that indicates the ordering of the configuration items of a resource.\"\n        }\n      ]\n    },\n    \"configurationItemMD5Hash\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationItemMD5Hash\"\n        },\n        {\n          \"description\": \"<p>Unique MD5 hash that represents the configuration item's state.</p> <p>You can use MD5 hash to compare the states of two or more configuration items that are associated with the same resource.</p>\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"Amazon\
  \ Resource Name (ARN) associated with the resource.\"\n        }\n      ]\n    },\n    \"resourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceType\"\n        },\n        {\n          \"description\": \"The type of Amazon Web Services resource.\"\n        }\n      ]\n    },\n    \"resourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The ID of the resource (for example, <code>sg-xxxxxx</code>).\"\n        }\n      ]\n    },\n    \"resourceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The custom name of the resource, if available.\"\n        }\n      ]\n    },\n    \"awsRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsRegion\"\n        },\n        {\n          \"description\": \"The region where\
  \ the resource resides.\"\n        }\n      ]\n    },\n    \"availabilityZone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AvailabilityZone\"\n        },\n        {\n          \"description\": \"The Availability Zone associated with the resource.\"\n        }\n      ]\n    },\n    \"resourceCreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceCreationTime\"\n        },\n        {\n          \"description\": \"The time stamp when the resource was created.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"A mapping of key value tags associated with the resource.\"\n        }\n      ]\n    },\n    \"relatedEvents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RelatedEventList\"\n        },\n        {\n          \"description\": \"<p>A list of CloudTrail\
  \ event IDs.</p> <p>A populated field indicates that the current configuration was initiated by the events recorded in the CloudTrail log. For more information about CloudTrail, see <a href=\\\"https://docs.aws.amazon.com/awscloudtrail/latest/userguide/what_is_cloud_trail_top_level.html\\\">What Is CloudTrail</a>.</p> <p>An empty field indicates that the current configuration was not initiated by any event. As of Version 1.3, the relatedEvents field is empty. You can access the <a href=\\\"https://docs.aws.amazon.com/awscloudtrail/latest/APIReference/API_LookupEvents.html\\\">LookupEvents API</a> in the <i>CloudTrail API Reference</i> to retrieve the events for the resource.</p>\"\n        }\n      ]\n    },\n    \"relationships\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RelationshipList\"\n        },\n        {\n          \"description\": \"A list of related Amazon Web Services resources.\"\n        }\n      ]\n    },\n    \"configuration\": {\n  \
  \    \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Configuration\"\n        },\n        {\n          \"description\": \"The description of the resource configuration.\"\n        }\n      ]\n    },\n    \"supplementaryConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SupplementaryConfiguration\"\n        },\n        {\n          \"description\": \"Configuration attributes that Config returns for certain resource types to supplement the information returned for the <code>configuration</code> parameter.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-configuration-item-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ConfigurationItem
---
