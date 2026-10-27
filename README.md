# 14.Grafana

# Задание 1
![1](https://github.com/ryltsevavikyla-coder/14.Grafana/blob/main/Screenshot%202026-10-27%20132731.png)

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

![2](https://github.com/ryltsevavikyla-coder/14.Grafana/blob/main/Screenshot%202026-10-27%20134019.png)

# Задание 3
![3](https://github.com/ryltsevavikyla-coder/14.Grafana/blob/main/Screenshot%202026-10-27%20135343.png)


# Задание 4
## JSON Model дашборда:
![2](https://github.com/ryltsevavikyla-coder/14.Grafana/blob/main/dashboard.json)
