# 14.Grafana



# Задание 2
# PromQL-запросы:
### CPU Utilization %
100 - (avg by (instance) (rate(node_cpu_seconds_total{mode="idle"}[5m])) * 100)

### Load Average
node_load1
node_load5
node_load15

### Free RAM
node_memory_MemAvailable_bytes

### Filesystem Free Space %
(node_filesystem_avail_bytes{fstype!~"tmpfs|overlay"} / node_filesystem_size_bytes{fstype!~"tmpfs|overlay"}) * 100
