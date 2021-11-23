# Zeebe Simple Monitor Helm Chart

Helm chart for simple monitor, the monitoring application for [Zeebe](https://zeebe.io). It is designed for developers to
* get in touch with Zeebe and workflow execution (BPMN)
* test workflows manually
* provide insides on how workflows are executed 

## Requirements

* [Helm](https://helm.sh/) >= 3.x +
* Kubernetes >= 1.18
* Hazelcast deployed
* Zeebe 1.x deployed
* Minimum cluster requirements include the following to run this chart with default settings. All of these settings are configurable.
  * 1GB of RAM for the JVM heap

 ## Configuration
  | Parameter                     | Description                                                                                                                                                                                                                                                                                                                | Default                                                                                                                   |
| ----------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| `global.zeebe.host`       | Zeebe broker host contact point | `zeebe-gateway` |
| `global.zeebe.host`       | Zeebe broker port contact point | `26500` |
| `env`                     | Array of env variables, check the `values-hazelcast.yaml` and `values-postgresql.yaml` for samples  | `[]` |


