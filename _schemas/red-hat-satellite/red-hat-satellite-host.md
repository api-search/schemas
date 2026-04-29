---
description: A host registered with Red Hat Satellite representing a physical, virtual, or cloud system.
layout: schema
name: Host
properties_list:
- description: Unique identifier for the host.
  name: id
  type: integer
- description: Fully qualified domain name (FQDN) of the host.
  name: name
  type: string
- description: Primary IPv4 address of the host.
  name: ip
  type: '[''string'', ''null'']'
- description: Primary IPv6 address of the host.
  name: ip6
  type: '[''string'', ''null'']'
- description: Primary MAC address of the host.
  name: mac
  type: '[''string'', ''null'']'
- description: Puppet environment identifier.
  name: environment_id
  type: '[''integer'', ''null'']'
- description: Host group identifier.
  name: hostgroup_id
  type: '[''integer'', ''null'']'
- description: Host group name.
  name: hostgroup_name
  type: '[''string'', ''null'']'
- description: Full host group title including parent groups.
  name: hostgroup_title
  type: '[''string'', ''null'']'
- description: Operating system identifier.
  name: operatingsystem_id
  type: '[''integer'', ''null'']'
- description: Operating system name and version.
  name: operatingsystem_name
  type: '[''string'', ''null'']'
- description: Architecture identifier.
  name: architecture_id
  type: '[''integer'', ''null'']'
- description: Architecture name (e.g., x86_64).
  name: architecture_name
  type: '[''string'', ''null'']'
- description: DNS domain identifier.
  name: domain_id
  type: '[''integer'', ''null'']'
- description: DNS domain name.
  name: domain_name
  type: '[''string'', ''null'']'
- description: IPv4 subnet identifier.
  name: subnet_id
  type: '[''integer'', ''null'']'
- description: IPv4 subnet name.
  name: subnet_name
  type: '[''string'', ''null'']'
- description: IPv6 subnet identifier.
  name: subnet6_id
  type: '[''integer'', ''null'']'
- description: Compute resource identifier. Null for bare metal hosts.
  name: compute_resource_id
  type: '[''integer'', ''null'']'
- description: Compute resource name.
  name: compute_resource_name
  type: '[''string'', ''null'']'
- description: Compute profile identifier.
  name: compute_profile_id
  type: '[''integer'', ''null'']'
- description: Installation medium identifier.
  name: medium_id
  type: '[''integer'', ''null'']'
- description: Partition table identifier.
  name: ptable_id
  type: '[''integer'', ''null'']'
- description: Hardware model identifier.
  name: model_id
  type: '[''integer'', ''null'']'
- description: Hardware model name.
  name: model_name
  type: '[''string'', ''null'']'
- description: Location identifier.
  name: location_id
  type: integer
- description: Location name.
  name: location_name
  type: string
- description: Organization identifier.
  name: organization_id
  type: integer
- description: Organization name.
  name: organization_name
  type: string
- description: Owner identifier.
  name: owner_id
  type: '[''integer'', ''null'']'
- description: Owner type (User or Usergroup).
  name: owner_type
  type: '[''string'', ''null'']'
- description: Whether the host is managed by Satellite for provisioning and configuration.
  name: managed
  type: boolean
- description: Whether the host is in build mode.
  name: build
  type: boolean
- description: Whether configuration management reports are evaluated for this host.
  name: enabled
  type: boolean
- description: Additional information about the host.
  name: comment
  type: '[''string'', ''null'']'
- description: Unique identifier from compute resource.
  name: uuid
  type: '[''string'', ''null'']'
- description: Global status of the host (0=OK, 1=Warning, 2=Error).
  name: global_status
  type: integer
- description: Human-readable global status label.
  name: global_status_label
  type: string
- description: Content-related attributes from the Katello content facet.
  name: content_facet_attributes
  type: object
- description: Subscription-related attributes from the Katello subscription facet.
  name: subscription_facet_attributes
  type: object
- description: Network interfaces associated with the host.
  name: interfaces
  type: array
- description: ''
  name: puppetclasses
  type: array
- description: ''
  name: all_puppetclasses
  type: array
- description: Timestamp when the host was created.
  name: created_at
  type: string
- description: Timestamp when the host was last updated.
  name: updated_at
  type: string
- description: Timestamp when the host OS was installed.
  name: installed_at
  type: '[''string'', ''null'']'
- description: Timestamp of the last configuration management report.
  name: last_report
  type: '[''string'', ''null'']'
provider_name: Red Hat Satellite
provider_slug: red-hat-satellite
schema_file: json-schema/red-hat-satellite-host-schema.json
slug: red-hat-satellite-host
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Host\",\n  \"type\": \"object\",\n  \"description\": \"A host registered with Red Hat Satellite representing a physical, virtual, or cloud system.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the host.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified domain name (FQDN) of the host.\"\n    },\n    \"ip\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Primary IPv4 address of the host.\"\n    },\n    \"ip6\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Primary IPv6 address of the host.\"\n    },\n    \"mac\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Primary MAC address of the host.\"\n    },\n    \"environment_id\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"Puppet environment\
  \ identifier.\"\n    },\n    \"hostgroup_id\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"Host group identifier.\"\n    },\n    \"hostgroup_name\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Host group name.\"\n    },\n    \"hostgroup_title\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Full host group title including parent groups.\"\n    },\n    \"operatingsystem_id\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"Operating system identifier.\"\n    },\n    \"operatingsystem_name\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Operating system name and version.\"\n    },\n    \"architecture_id\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"Architecture identifier.\"\n    },\n    \"architecture_name\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Architecture name (e.g., x86_64).\"\n    },\n    \"domain_id\": {\n\
  \      \"type\": \"['integer', 'null']\",\n      \"description\": \"DNS domain identifier.\"\n    },\n    \"domain_name\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"DNS domain name.\"\n    },\n    \"subnet_id\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"IPv4 subnet identifier.\"\n    },\n    \"subnet_name\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"IPv4 subnet name.\"\n    },\n    \"subnet6_id\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"IPv6 subnet identifier.\"\n    },\n    \"compute_resource_id\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"Compute resource identifier. Null for bare metal hosts.\"\n    },\n    \"compute_resource_name\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Compute resource name.\"\n    },\n    \"compute_profile_id\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"Compute profile\
  \ identifier.\"\n    },\n    \"medium_id\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"Installation medium identifier.\"\n    },\n    \"ptable_id\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"Partition table identifier.\"\n    },\n    \"model_id\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"Hardware model identifier.\"\n    },\n    \"model_name\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Hardware model name.\"\n    },\n    \"location_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Location identifier.\"\n    },\n    \"location_name\": {\n      \"type\": \"string\",\n      \"description\": \"Location name.\"\n    },\n    \"organization_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Organization identifier.\"\n    },\n    \"organization_name\": {\n      \"type\": \"string\",\n      \"description\": \"Organization name.\"\n    },\n    \"owner_id\":\
  \ {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"Owner identifier.\"\n    },\n    \"owner_type\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Owner type (User or Usergroup).\"\n    },\n    \"managed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the host is managed by Satellite for provisioning and configuration.\"\n    },\n    \"build\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the host is in build mode.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether configuration management reports are evaluated for this host.\"\n    },\n    \"comment\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Additional information about the host.\"\n    },\n    \"uuid\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Unique identifier from compute resource.\"\n    },\n    \"global_status\": {\n      \"type\": \"integer\",\n \
  \     \"description\": \"Global status of the host (0=OK, 1=Warning, 2=Error).\"\n    },\n    \"global_status_label\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable global status label.\"\n    },\n    \"content_facet_attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Content-related attributes from the Katello content facet.\"\n    },\n    \"subscription_facet_attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Subscription-related attributes from the Katello subscription facet.\"\n    },\n    \"interfaces\": {\n      \"type\": \"array\",\n      \"description\": \"Network interfaces associated with the host.\"\n    },\n    \"puppetclasses\": {\n      \"type\": \"array\"\n    },\n    \"all_puppetclasses\": {\n      \"type\": \"array\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the host was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n    \
  \  \"description\": \"Timestamp when the host was last updated.\"\n    },\n    \"installed_at\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Timestamp when the host OS was installed.\"\n    },\n    \"last_report\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Timestamp of the last configuration management report.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat-satellite/refs/heads/main/json-schema/red-hat-satellite-host-schema.json
tags:
- Configuration Management
- Lifecycle Management
- Patch Management
- Subscription Management
- Systems Management
title: Host
---
