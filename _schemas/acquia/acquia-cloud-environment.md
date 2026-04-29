---
description: environment schema from Acquia Cloud API
layout: schema
name: Environment
properties_list:
- description: The ID of the environment. The ID is a compound key consisting of the internal database ID of the environment and the application UUID.
  name: id
  type: string
- description: The human-readable name of the environment.
  name: label
  type: string
- description: The stage name of the environment.
  name: name
  type: string
- description: ''
  name: application
  type: object
- description: An array of domain names attached to this environment.
  name: domains
  type: array
- description: The active domain name for this environment.
  name: active_domain
  type: string
- description: The default domain name for this environment.
  name: default_domain
  type: string
- description: The URL to the image for this environment.
  name: image_url
  type: string
- description: The URL used to SSH into the environment.
  name: ssh_url
  type: string
- description: An array of IP addresses attached to this environment.
  name: ips
  type: array
- description: The region the environment resides in.
  name: region
  type: string
- description: 'The balancer type. - balancers: The environment is behind a Legacy balancer. - elb: The environment is behind an ELB balancer. - cluster: The environment is behind an Edge Cluster balancer.'
  name: balancer
  type: string
- description: 'The platform type. - cloud: The environment is hosted on a Cloud Classic Platform. - cloud-next: The environment is hosted on a Cloud Next Platform. - unknown: The host information is not available fo'
  name: platform
  type: string
- description: The status of this environment.
  name: status
  type: string
- description: 'The type of environment. - node: A NodeJS environment. - drupal: A Drupal environment. - ssg: A Static Site Generator environment. - unknown: We were unable to determine the environment type.'
  name: type
  type: string
- description: The size of the environment. Will be null if the environment type does not support sizes.
  name: size
  type: string
- description: The environment weight for display purposes.
  name: weight
  type: integer
- description: ''
  name: vcs
  type: object
- description: ''
  name: flags
  type: object
- description: A collection of environment configuration information.
  name: configuration
  type: object
- description: ''
  name: artifact
  type: object
- description: ''
  name: _links
  type: object
provider_name: Acquia
provider_slug: acquia
schema_file: json-schema/acquia-cloud-environment-schema.json
slug: acquia-cloud-environment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-environment-schema.json\",\n  \"title\": \"Environment\",\n  \"description\": \"environment schema from Acquia Cloud API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the environment. The ID is a compound key consisting of the internal database ID of the environment and the application UUID.\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable name of the environment.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The stage name of the environment.\"\n    },\n    \"application\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_application-stub\"\n    },\n    \"domains\": {\n      \"type\": \"array\",\n      \"\
  description\": \"An array of domain names attached to this environment.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"hostname\"\n      }\n    },\n    \"active_domain\": {\n      \"type\": \"string\",\n      \"format\": \"hostname\",\n      \"description\": \"The active domain name for this environment.\"\n    },\n    \"default_domain\": {\n      \"type\": \"string\",\n      \"format\": \"hostname\",\n      \"description\": \"The default domain name for this environment.\"\n    },\n    \"image_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to the image for this environment.\",\n      \"nullable\": true\n    },\n    \"ssh_url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL used to SSH into the environment.\"\n    },\n    \"ips\": {\n      \"type\": \"array\",\n      \"description\": \"An array of IP addresses attached to this environment.\",\n      \"deprecated\": true,\n      \"items\"\
  : {\n        \"type\": \"string\",\n        \"format\": \"ipv4\"\n      }\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The region the environment resides in.\"\n    },\n    \"balancer\": {\n      \"type\": \"string\",\n      \"description\": \"The balancer type.\\n- balancers: The environment is behind a Legacy balancer.\\n- elb: The environment is behind an ELB balancer.\\n- cluster: The environment is behind an Edge Cluster balancer.\\n\",\n      \"enum\": [\n        \"balancers\",\n        \"elb\",\n        \"cluster\"\n      ]\n    },\n    \"platform\": {\n      \"type\": \"string\",\n      \"description\": \"The platform type.\\n- cloud: The environment is hosted on a Cloud Classic Platform.\\n- cloud-next: The environment is hosted on a Cloud Next Platform.\\n- unknown:  The host information is not available for the environment.\\n\",\n      \"enum\": [\n        \"cloud\",\n        \"cloud-next\",\n        \"unknown\"\n      ]\n    },\n    \"\
  status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of this environment.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of environment.\\n- node: A NodeJS environment.\\n- drupal: A Drupal environment.\\n- ssg: A Static Site Generator environment.\\n- unknown: We were unable to determine the environment type.\\n\",\n      \"enum\": [\n        \"node\",\n        \"drupal\",\n        \"ssg\",\n        \"unknown\"\n      ]\n    },\n    \"size\": {\n      \"type\": \"string\",\n      \"description\": \"The size of the environment. Will be null if the environment type does not support sizes.\",\n      \"nullable\": true,\n      \"enum\": [\n        \"small\",\n        \"medium\",\n        \"large\",\n        \"unknown\"\n      ]\n    },\n    \"weight\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"The environment weight for display purposes.\"\n    },\n    \"vcs\": {\n      \"$ref\"\
  : \"#/components/schemas/Acquia_Cloud_API_Documentation_vcs\"\n    },\n    \"flags\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_environment-flags\"\n    },\n    \"configuration\": {\n      \"type\": \"object\",\n      \"description\": \"A collection of environment configuration information.\",\n      \"nullable\": true,\n      \"properties\": {\n        \"operating_system\": {\n          \"type\": \"string\",\n          \"description\": \"The environment operation system.\"\n        },\n        \"php\": {\n          \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_environment-configuration\"\n        }\n      }\n    },\n    \"artifact\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_artifact-stub\"\n    },\n    \"_links\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_links\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"label\",\n    \"name\",\n    \"application\",\n    \"domains\"\
  ,\n    \"active_domain\",\n    \"default_domain\",\n    \"image_url\",\n    \"ssh_url\",\n    \"ips\",\n    \"region\",\n    \"balancer\",\n    \"platform\",\n    \"status\",\n    \"type\",\n    \"size\",\n    \"weight\",\n    \"vcs\",\n    \"flags\",\n    \"configuration\",\n    \"artifact\",\n    \"_links\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-environment-schema.json
tags:
- Content
- Experience
title: Environment
---
