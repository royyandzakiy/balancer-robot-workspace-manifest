# 1. Initialize the workspace using this workspace-manifest, rename generated parent workspace folder
```bash
west init -m https://github.com/royyandzakiy/balancer-robot-workspace-manifest.git balancer-robot-workspace
```

```bash
cd balancer-robot-workspace
```

# 3. Pull all repos (Zephyr, FW, and Desktop App)
```bash
west update
```