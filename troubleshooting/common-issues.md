# Common Issues & Resolutions

## 1. Permission Denied Errors

Issue:
Container unable to access mounted volume.

Cause:
Incorrect ownership or root-owned directory.

Fix:
Use chown to correct UID/GID.
Verify container user permissions.

---

## 2. Bad Gateway (502) from Reverse Proxy

Issue:
Nginx Proxy Manager shows 502 error.

Cause:
Target container not running or wrong internal port.

Fix:
Check container status with:
docker ps

Verify service port configuration.

---

## 3. Monitoring Not Displaying Metrics

Issue:
Grafana shows no data.

Cause:
Prometheus target misconfigured.

Fix:
Verify scrape targets in prometheus.yml.
Restart Prometheus container.
