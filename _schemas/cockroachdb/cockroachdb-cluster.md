---
description: Schema representing a CockroachDB Cloud cluster, which is an instance of CockroachDB running in one or more cloud regions on Serverless or Dedicated infrastructure.
layout: schema
name: CockroachDB Cluster
properties_list:
- description: Unique identifier of the cluster assigned by CockroachDB Cloud.
  name: id
  type: string
- description: Human-readable name of the cluster.
  name: name
  type: string
- description: Cloud infrastructure provider hosting the cluster.
  name: cloud_provider
  type: string
- description: Version string of CockroachDB running on the cluster (e.g. v23.1.0).
  name: cockroach_version
  type: string
- description: Service tier of the cluster, either Serverless or Dedicated.
  name: plan
  type: string
- description: Overall lifecycle state of the cluster.
  name: state
  type: string
- description: Current operational status reflecting any in-progress or failed operations.
  name: operation_status
  type: string
- description: Cloud provider regions where the cluster is deployed. Multi-region clusters have multiple entries.
  name: regions
  type: array
- description: Configuration settings for the cluster, containing either serverless or dedicated configuration.
  name: config
  type: object
- description: Identifier of the user who created the cluster.
  name: creator_id
  type: string
- description: RFC3339 timestamp when the cluster was created.
  name: created_at
  type: string
- description: RFC3339 timestamp of the most recent modification to the cluster.
  name: updated_at
  type: string
- description: RFC3339 timestamp when the cluster was deleted. Only present for deleted clusters.
  name: deleted_at
  type: string
- description: DNS hostname used for SQL connections to the cluster.
  name: sql_dns
  type: string
- description: Status of any in-progress version upgrade operation.
  name: upgrade_status
  type: string
- description: Cloud provider account ID for the cluster, used for trust relationship configuration.
  name: account_id
  type: string
- description: Folder ID of the folder containing this cluster, if any.
  name: parent_id
  type: string
- description: User-defined key-value labels attached to the cluster for organization and filtering.
  name: labels
  type: object
- description: Whether delete protection is enabled, preventing accidental cluster deletion.
  name: delete_protection
  type: string
- description: Policy governing outbound network traffic from the cluster.
  name: egress_traffic_policy
  type: string
- description: Network accessibility configuration controlling whether the cluster is publicly accessible.
  name: network_visibility
  type: string
- description: Client ID of the Azure cluster identity, present for Azure deployments that support CMEK.
  name: azure_cluster_identity_client_id
  type: string
- description: IPv4 CIDR range reserved for the cluster. Only set on GCP Advanced tier clusters.
  name: cidr_range
  type: string
- description: Customer cloud account details for BYOC (Bring Your Own Cloud) deployments.
  name: customer_cloud_account
  type: object
provider_name: CockroachDB
provider_slug: cockroachdb
schema_file: json-schema/cockroachdb-cluster-schema.json
slug: cockroachdb-cluster
tags:
- Cluster Management
- Cloud
- Database
- Distributed SQL
- Infrastructure
- PostgreSQL Compatible
- SQL
title: CockroachDB Cluster
---
