# Developer Guide

There's a `Makefile` in the root folder. Here are some common options:

Build all binaries (`yurt-controller-manager`, `yurthub`, `yurtadm`)
```bash
make build
```

Build specific binary for specific architecture. (`amd64`,`arm`,`arm64`)
```bash
GOOS=linux GOARCH=arm64 make build WHAT=cmd/yurtadm
```

Build all docker images for all supported architectures.
```bash
make release
```

Build all docker images for specific architecture.
```bash
make release ARCH=arm64
```

Build yurt-e2e-test binary to test Openyurt.
```bash
make e2e
```

Please check [yurt-e2e-test tutorial](./tutorial/yurt-e2e-test.md) for more details.
Please check [yurt-app-manager dev tutorial](./tutorial/yurt-app-manager-dev.md) for more details.
