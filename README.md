# DevOps Task 7: Monitor System Resources Using Netdata

## Objective
Install and use Netdata to monitor system and application performance metrics in real-time using Docker.

## Tools Used
- Docker
- Netdata (Docker image)

## Steps Followed
1. Pulled and ran the Netdata Docker container using the command:
   ```bash
   docker run -d --name=netdata -p 19999:19999 --cap-add SYS_PTRACE --security-opt apparmor=unconfined netdata/netdata
   ```

2. Opened Netdata dashboard at [http://localhost:19999](http://localhost:19999)

3. Monitored various system metrics such as:
   - CPU usage
   - Memory usage
   - Disk I/O
   - Network throughput
   - Docker container stats

## Screenshot
Please add your dashboard screenshot here (e.g., screenshot.png)

## Interview Questions

### 1. What does Netdata monitor?
Netdata monitors CPU, memory, disk usage, network, processes, Docker containers, and more.

### 2. How do you view real-time metrics?
By accessing the dashboard at `http://localhost:19999` in a browser.

### 3. How is Netdata different from Prometheus?
Netdata is plug-and-play with real-time visualization. Prometheus is ideal for time-series storage and requires configuration.

### 4. What is a collector?
A collector in Netdata is a plugin or agent that gathers specific metrics.

### 5. What are some performance KPIs to watch?
CPU load, memory usage, disk I/O, network traffic, and container resource utilization.

### 6. How to deploy Netdata on a VM?
Either using Docker or by installing the Netdata agent directly on the VM.

### 7. How does Netdata alerting work?
Netdata uses pre-configured alarm thresholds and can send notifications via email, Slack, webhooks, etc.

### 8. What is a dashboard in this context?
A web-based UI that displays real-time monitoring data and charts for various system metrics.

