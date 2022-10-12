# Elasticsearch-Kibana Docker Compose
It contains docker instances for both **Elasticsearch** & **Kibana** internally connected via bridge network.

### Elasticsearch
Elasticsearch, the search engine itself can be accessed on host machine (localhost) on port _9200_.

#### Description
Below configuration are already set by default via `esCreds.env` file and can be modified by overriding the same.

| Config   | Value    | Comment                                                       |
| -------- | -------- | ------------------------------------------------------------- |
| Port     | 9200     | Exposed at localhost (127.0.0.1)                              |
| Username | elastic  |                                                               |
| Password |          | Passowrd is disabled via `xpack.security.enabled:false`       |
| RAM      | 2 GB     | Memory is restricted to 2 GB via `bootstrap.memory_lock:true` |

### Kibana
Kibana is integrated to graphically visualize the elasticsearch.
It can be accessed on host machine (localhost) web browser at http://localhost:5601.

#### Configuration
Below configuration are already set by default via `kibanaCreds.env` file and can be modified by overriding the same.

| Config   | Value | Comment                          |
| -------- | ----- | -------------------------------- |
| Port     | 5601  | Exposed at localhost (127.0.0.1) |
