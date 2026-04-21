---
description: Credit monitoring enrollment record for a consumer.
layout: schema
name: MonitoringEnrollment
properties_list:
- description: Unique identifier for the monitoring enrollment.
  name: enrollment_id
  type: string
- description: Consumer this enrollment belongs to.
  name: consumer_id
  type: string
- description: Enrollment status.
  name: status
  type: string
- description: Bureaus being monitored.
  name: bureaus
  type: array
- description: ''
  name: created_at
  type: string
provider_name: Bloom Credit
provider_slug: bloom-credit
schema_file: json-schema/bloom-credit-monitoring-enrollment-schema.json
slug: bloom-credit-monitoring-enrollment
tags:
- Credit Bureau
- Credit Reports
- Credit Scores
- Fintech
- Lending
- Personal Finance
title: MonitoringEnrollment
---
