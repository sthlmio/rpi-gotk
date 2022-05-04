# rpi-gotk

GitOps repo for Flux v2 running on our Raspberry Pi Kubernetes cluster.

## Hardware (cluster)

Raspberry Pi cluster containing of:

- Raspberry Pi 4 8 GB nodes
- HA: 3 master nodes and 3 worker nodes
- PoE+ HAT on each node for power and network
- SSD disk attached to each node
- Ubiquiti UniFi USG and MetalLB as load-balancer

| NAME | ROLES                     | VERSION      |
| ---- | ------------------------- | ------------ |
| rp0  | control-plane,etcd,master | v1.23.6+k3s1 |
| rp1  | control-plane,etcd,master | v1.23.6+k3s1 |
| rp2  | control-plane,etcd,master | v1.23.6+k3s1 |
| rp3  | worker                    | v1.23.6+k3s1 |
| rp4  | worker                    | v1.23.6+k3s1 |
| rp5  | worker                    | v1.23.6+k3s1 |

## Documentation

See [DOCUMENTATION.md](./DOCUMENTATION.md) for docs.
