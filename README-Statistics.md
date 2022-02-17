# ProxySQL Statistics

## Introduction

If you followed this [workshop on ProxySQL](README.md) you should have a working ProxySQL server. ProxySQL collects a lot of real time statistics in the stats schema, each table provides specific information about the behaviour of ProxySQL and the workload being processed. We'll go over some of the statistics at our disposal.

![Architecture](images/architecture.png)  

## Requirements:

* Working ProxySQL server.

## ProxySQL Statistics

### The `stats schema`

Those are the tables at our disposal. Each table provides specific information about the behavior of ProxySQL and the workload being processed.

```sql
SHOW TABLES FROM stats;
```

      +--------------------------------------+
      | tables                               |
      +--------------------------------------+
      | global_variables                     |
      | stats_memory_metrics                 |
      | stats_mysql_client_host_cache        |
      | stats_mysql_client_host_cache_reset  |
      | stats_mysql_commands_counters        |
      | stats_mysql_connection_pool          |
      | stats_mysql_connection_pool_reset    |
      | stats_mysql_errors                   |
      | stats_mysql_errors_reset             |
      | stats_mysql_free_connections         |
      | stats_mysql_global                   |
      | stats_mysql_gtid_executed            |
      | stats_mysql_prepared_statements_info |
      | stats_mysql_processlist              |
      | stats_mysql_query_digest             |
      | stats_mysql_query_digest_reset       |
      | stats_mysql_query_rules              |
      | stats_mysql_users                    |
      | stats_proxysql_servers_checksums     |
      | stats_proxysql_servers_metrics       |
      | stats_proxysql_servers_status        |
      +--------------------------------------+
      21 rows in set (0.003 sec)


## Useful Links

Nice and useful links.

- [ProxySQL Initial Configuration](https://proxysql.com/documentation/ProxySQL-Configuration/)
- [Nice MySQL training](https://www.mysqltutorial.org/)

## License

This project is licensed under the [MIT license](LICENSE).

[*^ back to top*](#ProxySQL-on-Docker)
