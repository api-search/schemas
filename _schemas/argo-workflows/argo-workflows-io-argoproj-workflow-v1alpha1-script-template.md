---
description: ScriptTemplate is a template subtype to enable scripting through code steps
layout: schema
name: io.argoproj.workflow.v1alpha1.ScriptTemplate
properties_list:
- description: Arguments to the entrypoint. The container image's CMD is used if this is not provided. Variable references $(VAR_NAME) are expanded using the container's environment. If a variable cannot be resolved
  name: args
  type: array
- description: Entrypoint array. Not executed within a shell. The container image's ENTRYPOINT is used if this is not provided. Variable references $(VAR_NAME) are expanded using the container's environment. If a va
  name: command
  type: array
- description: List of environment variables to set in the container. Cannot be updated.
  name: env
  type: array
- description: List of sources to populate environment variables in the container. The keys defined within a source may consist of any printable ASCII characters except '='. When a key exists in multiple sources, th
  name: envFrom
  type: array
- description: 'Container image name. More info: https://kubernetes.io/docs/concepts/containers/images This field is optional to allow higher level config management to default or override container images in workloa'
  name: image
  type: string
- description: 'Image pull policy. One of Always, Never, IfNotPresent. Defaults to Always if :latest tag is specified, or IfNotPresent otherwise. Cannot be updated. More info: https://kubernetes.io/docs/concepts/cont'
  name: imagePullPolicy
  type: string
- description: Actions that the management system should take in response to container lifecycle events. Cannot be updated.
  name: lifecycle
  type: object
- description: 'Periodic probe of container liveness. Container will be restarted if the probe fails. Cannot be updated. More info: https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes'
  name: livenessProbe
  type: object
- description: Name of the container specified as a DNS_LABEL. Each container in a pod must have a unique name (DNS_LABEL). Cannot be updated.
  name: name
  type: string
- description: List of ports to expose from the container. Not specifying a port here DOES NOT prevent that port from being exposed. Any port which is listening on the default "0.0.0.0" address inside a container wi
  name: ports
  type: array
- description: 'Periodic probe of container service readiness. Container will be removed from service endpoints if the probe fails. Cannot be updated. More info: https://kubernetes.io/docs/concepts/workloads/pods/pod'
  name: readinessProbe
  type: object
- description: Resources resize policy for the container. This field cannot be set on ephemeral containers.
  name: resizePolicy
  type: array
- description: 'Compute Resources required by this container. Cannot be updated. More info: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/'
  name: resources
  type: object
- description: RestartPolicy defines the restart behavior of individual containers in a pod. This overrides the pod-level restart policy. When this field is not specified, the restart behavior is defined by the Pod'
  name: restartPolicy
  type: string
- description: Represents a list of rules to be checked to determine if the container should be restarted on exit. The rules are evaluated in order. Once a rule matches a container exit condition, the remaining rule
  name: restartPolicyRules
  type: array
- description: 'SecurityContext defines the security options the container should be run with. If set, the fields of SecurityContext override the equivalent fields of PodSecurityContext. More info: https://kubernetes'
  name: securityContext
  type: object
- description: Source contains the source code of the script to execute
  name: source
  type: string
- description: 'StartupProbe indicates that the Pod has successfully initialized. If specified, no other probes are executed until this completes successfully. If this probe fails, the Pod will be restarted, just as '
  name: startupProbe
  type: object
- description: Whether this container should allocate a buffer for stdin in the container runtime. If this is not set, reads from stdin in the container will always result in EOF. Default is false.
  name: stdin
  type: boolean
- description: Whether the container runtime should close the stdin channel after it has been opened by a single attach. When stdin is true the stdin stream will remain open across multiple attach sessions. If stdin
  name: stdinOnce
  type: boolean
- description: 'Optional: Path at which the file to which the container''s termination message will be written is mounted into the container''s filesystem. Message written is intended to be brief final status, such as '
  name: terminationMessagePath
  type: string
- description: Indicate how the termination message should be populated. File will use the contents of terminationMessagePath to populate the container status message on both success and failure. FallbackToLogsOnErr
  name: terminationMessagePolicy
  type: string
- description: Whether this container should allocate a TTY for itself, also requires 'stdin' to be true. Default is false.
  name: tty
  type: boolean
- description: volumeDevices is the list of block devices to be used by the container.
  name: volumeDevices
  type: array
- description: Pod volumes to mount into the container's filesystem. Cannot be updated.
  name: volumeMounts
  type: array
- description: Container's working directory. If not specified, the container runtime's default will be used, which might be configured in the container image. Cannot be updated.
  name: workingDir
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-script-template-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-script-template
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ScriptTemplate
---
