### Required after package installation

It is necessary to create frr user in order to start frr.service

```bash
sudo useradd -M -l frr -s /sbin/nologin -d /var/lib/frr
sudo usermod -L frr
```

It is recommended to reload systemd daemon on each config file modification.
```bash
sudo systemctl daemon-reload
```
