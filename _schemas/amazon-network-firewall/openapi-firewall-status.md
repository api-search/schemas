---
description: Detailed information about the current status of a <a>Firewall</a>. You can retrieve this for a firewall by calling <a>DescribeFirewall</a> and providing the firewall name and ARN.
layout: schema
name: FirewallStatus
properties_list:
- description: ''
  name: Status
  type: object
- description: ''
  name: ConfigurationSyncStateSummary
  type: object
- description: ''
  name: SyncStates
  type: object
- description: ''
  name: CapacityUsageSummary
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-firewall-status-schema.json
slug: openapi-firewall-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-firewall-status-schema.json\",\n  \"title\": \"FirewallStatus\",\n  \"description\": \"Detailed information about the current status of a <a>Firewall</a>. You can retrieve this for a firewall by calling <a>DescribeFirewall</a> and providing the firewall name and ARN.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirewallStatusValue\"\n        },\n        {\n          \"description\": \"The readiness of the configured firewall to handle network traffic across all of the Availability Zones where you've configured it. This setting is <code>READY</code> only when the <code>ConfigurationSyncStateSummary</code> value is <code>IN_SYNC</code> and the <code>Attachment</code> <code>Status</code> values\
  \ for all of the configured subnets are <code>READY</code>. \"\n        }\n      ]\n    },\n    \"ConfigurationSyncStateSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationSyncState\"\n        },\n        {\n          \"description\": \"<p>The configuration sync state for the firewall. This summarizes the sync states reported in the <code>Config</code> settings for all of the Availability Zones where you have configured the firewall. </p> <p>When you create a firewall or update its configuration, for example by adding a rule group to its firewall policy, Network Firewall distributes the configuration changes to all zones where the firewall is in use. This summary indicates whether the configuration changes have been applied everywhere. </p> <p>This status must be <code>IN_SYNC</code> for the firewall to be ready for use, but it doesn't indicate that the firewall is ready. The <code>Status</code> setting indicates firewall readiness.</p>\"\
  \n        }\n      ]\n    },\n    \"SyncStates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyncStates\"\n        },\n        {\n          \"description\": \"The subnets that you've configured for use by the Network Firewall firewall. This contains one array element per Availability Zone where you've configured a subnet. These objects provide details of the information that is summarized in the <code>ConfigurationSyncStateSummary</code> and <code>Status</code>, broken down by zone and configuration object. \"\n        }\n      ]\n    },\n    \"CapacityUsageSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CapacityUsageSummary\"\n        },\n        {\n          \"description\": \"Describes the capacity usage of the resources contained in a firewall's reference sets. Network Firewall calclulates the capacity usage by taking an aggregated count of all of the resources used by all of the reference sets in a firewall.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Status\",\n    \"ConfigurationSyncStateSummary\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-firewall-status-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: FirewallStatus
---
