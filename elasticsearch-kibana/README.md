# Elasticsearch-Kibana Docker Compose
It contains docker instances for both **Elasticsearch** & **Kibana** internally connected via bridge network.

### Elasticsearch
Elasticsearch, the search engine itself can be accessed on host machine (localhost) on port _9200_.

#### Description
Below configuration are already set by default via `esCreds.env` file and can be modified by overriding the same.

| Config        | Value   | Comment                                                                  |
| ------------- | ------- | ------------------------------------------------------------------------ |
| Port          | 9200    | Exposed at localhost (127.0.0.1)                                         |
| Username      | elastic |                                                                          |
| Password      |         | Password is disabled via `xpack.security.enabled:false`                  |
| JVM Memory    | 2 GB    | JVM memory usage is constrained to 2 GB via `bootstrap.memory_lock:true` |
| Docker Memory | 3 GB    | Container's main memory usage is limited to 3 GB via compose file        |

### Kibana
Kibana is integrated to graphically visualize the elasticsearch.
It can be accessed on host machine (localhost) web browser at http://localhost:5601.

#### Configuration
Below configuration are already set by default via `kibanaCreds.env` file and can be modified by overriding the same.

| Config        | Value | Comment                                                           |
| ------------- | ----- | ----------------------------------------------------------------- |
| Port          | 5601  | Exposed at localhost (127.0.0.1)                                  |
| Docker Memory | 1 GB  | Container's main memory usage is limited to 1 GB via compose file |
