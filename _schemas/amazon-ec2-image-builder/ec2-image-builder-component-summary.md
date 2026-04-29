---
description: A high-level summary of a component.
layout: schema
name: ComponentSummary
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: version
  type: object
- description: ''
  name: platform
  type: object
- description: ''
  name: supportedOsVersions
  type: object
- description: ''
  name: state
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: owner
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: changeDescription
  type: object
- description: ''
  name: dateCreated
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: publisher
  type: object
- description: ''
  name: obfuscate
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-component-summary-schema.json
slug: ec2-image-builder-component-summary
source_filename: ec2-image-builder-component-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-component-summary-schema.json\",\n  \"title\": \"ComponentSummary\",\n  \"description\": \"A high-level summary of a component.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuilderArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the component.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceName\"\n        },\n        {\n          \"description\": \"The name of the component.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionNumber\"\n        },\n        {\n          \"description\"\
  : \"The version of the component.\"\n        }\n      ]\n    },\n    \"platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Platform\"\n        },\n        {\n          \"description\": \"The operating system platform of the component.\"\n        }\n      ]\n    },\n    \"supportedOsVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OsVersionList\"\n        },\n        {\n          \"description\": \"The operating system (OS) version that the component supports. If the OS information is available, Image Builder performs a prefix match against the base image OS version during image recipe creation.\"\n        }\n      ]\n    },\n    \"state\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentState\"\n        },\n        {\n          \"description\": \"Describes the current status of the component.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/ComponentType\"\n        },\n        {\n          \"description\": \"The component type specifies whether Image Builder uses the component to build the image or only to test it.\"\n        }\n      ]\n    },\n    \"owner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The owner of the component.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The description of the component.\"\n        }\n      ]\n    },\n    \"changeDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The change description for the current version of the component.\"\n        }\n      ]\n    },\n    \"dateCreated\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The original creation date of the component.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags that apply to the component.\"\n        }\n      ]\n    },\n    \"publisher\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"Contains the name of the publisher if this is a third-party component. Otherwise, this property is empty.\"\n        }\n      ]\n    },\n    \"obfuscate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Indicates whether component source is hidden from view in the console, and from component detail results\
  \ for API, CLI, or SDK operations.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-component-summary-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ComponentSummary
---
