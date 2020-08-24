
# snowflake_warehouse

<!-- These docs are auto-generated by code in ./docgen, run by with make docs. Manual edits will be overwritten. -->

## properties

|             NAME             |  TYPE  |                                                               DESCRIPTION                                                                | OPTIONAL | REQUIRED  | COMPUTED | DEFAULT |
|------------------------------|--------|------------------------------------------------------------------------------------------------------------------------------------------|----------|-----------|----------|---------|
| auto_resume                  | bool   | Specifies whether to automatically resume a warehouse when a SQL statement (e.g. query) is submitted to it.                              | true     | false     | true     |         |
| auto_suspend                 | int    | Specifies the number of seconds of inactivity after which a warehouse is automatically suspended.                                        | true     | false     | true     |         |
| comment                      | string |                                                                                                                                          | true     | false     | false    | ""      |
| initially_suspended          | bool   | Specifies whether the warehouse is created initially in the ‘Suspended’ state.                                                           | true     | false     | false    |         |
| max_cluster_count            | int    | Specifies the maximum number of server clusters for the warehouse.                                                                       | true     | false     | true     |         |
| min_cluster_count            | int    | Specifies the minimum number of server clusters for the warehouse (only applies to multi-cluster warehouses).                            | true     | false     | true     |         |
| name                         | string |                                                                                                                                          | false    | true      | false    |         |
| resource_monitor             | string | Specifies the name of a resource monitor that is explicitly assigned to the warehouse.                                                   | true     | false     | true     |         |
| scaling_policy               | string | Specifies the policy for automatically starting and shutting down clusters in a multi-cluster warehouse running in Auto-scale mode.      | true     | false     | true     |         |
| statement_timeout_in_seconds | int    | Specifies the time, in seconds, after which a running SQL statement (query, DDL, DML, etc.) is canceled by the system                    | true     | false     | false    |       0 |
| wait_for_provisioning        | bool   | Specifies whether the warehouse, after being resized, waits for all the servers to provision before executing any queued or new queries. | true     | false     | false    |         |
| warehouse_size               | string |                                                                                                                                          | true     | false     | true     |         |