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
Please add your dashboard screenshot here (screenshot-1.png)

