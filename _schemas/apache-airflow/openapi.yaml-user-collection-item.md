---
description: A user object. *New in version 2.1.0*
layout: schema
name: UserCollectionItem
properties_list:
- description: Whether the user is active
  name: active
  type: boolean
- description: The date user was changed
  name: changed_on
  type: string
- description: The date user was created
  name: created_on
  type: string
- description: The user's email. *Changed in version 2.2.0*&#58; A minimum character length requirement ('minLength') is added.
  name: email
  type: string
- description: The number of times the login failed
  name: failed_login_count
  type: integer
- description: The user's first name. *Changed in version 2.4.0*&#58; The requirement for this to be non-empty was removed.
  name: first_name
  type: string
- description: The last user login
  name: last_login
  type: string
- description: The user's last name. *Changed in version 2.4.0*&#58; The requirement for this to be non-empty was removed.
  name: last_name
  type: string
- description: The login count
  name: login_count
  type: integer
- description: User roles. *Changed in version 2.2.0*&#58; Field is no longer read-only.
  name: roles
  type: array
- description: The username. *Changed in version 2.2.0*&#58; A minimum character length requirement ('minLength') is added.
  name: username
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-user-collection-item-schema.json
slug: openapi.yaml-user-collection-item
tags:
- Apache
- DAG
- Data Pipeline
- ETL
- Open Source
- Orchestration
- Python
- Scheduling
- Workflow
title: UserCollectionItem
---
