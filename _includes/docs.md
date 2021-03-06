## APIs

1. Enroll nodes by creating `BareMetalHost` resources.  This would either be
   manually or done by a component doing node discovery and introspection.

   See the documentation in the
   [baremetal-operator](https://github.com/metal3-io/baremetal-operator/blob/master/docs/api.md) repository for details.

2. Use the machine API to allocate a machine.

   See the documentation in the
   [cluster-api-provider-baremetal](https://github.com/metal3-io/cluster-api-provider-baremetal/blob/master/docs/api.md)
   repository for details.

3. The new Machine is associated with an available `BareMetalHost`, which triggers
   provisioning of that host to join the cluster.  This association is done by
   the Actuator when it sets the `MachineRef` field on the `BareMetalHost`.

## Design Documents

The design documents for Metal3 are all publicly available. Refer to the [metal3-io/metal3-docs github repository](https://github.com/metal3-io/metal3-docs) for details.

## Around the Web

### Conference Talks

- [Extend Your Data Center to the Hybrid Edge - Red Hat Summit, May 2019](https://www.pscp.tv/RedHatOfficial/1vAGRWYPjngJl?t=1h27m51s)
- [OpenStack Ironic and Bare Metal Infrastructure: All Abstractions Start Somewhere - Chris Hoge, OpenStack Foundation; Julia Kreger, Red Hat](https://www.openstack.org/summit/denver-2019/summit-schedule/events/23779/openstack-ironic-and-bare-metal-infrastructure-all-abstractions-start-somewhere)
- [Kubernetes-native Infrastructure: Managed Baremetal with Kubernetes Operators and OpenStack Ironic - Steve Hardy, Red Hat](https://sched.co/KMyE)

### In The News

- [The New Stack: Metal3 Uses OpenStack’s Ironic for Declarative Bare Metal Kubernetes](https://thenewstack.io/metal3-uses-openstacks-ironic-for-declarative-bare-metal-kubernetes/)
- [The Register: Raise some horns: Red Hat's MetalKube aims to make Kubernetes on bare machines simple](https://www.theregister.co.uk/2019/04/05/red_hat_metalkubel/)

### Blog Posts

- [Metal³ Blog posts](/blog/)
