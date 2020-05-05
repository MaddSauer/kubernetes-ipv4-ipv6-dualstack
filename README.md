# IPv4 / IPv6 Dualstack on K8s

## public documentation

calico:
  * https://www.projectcalico.org/dual-stack-operation-with-calico-on-kubernetes
  * https://docs.projectcalico.org/networking/ipv6#modifying-your-dns-for-ipv6

## summary
  * you must run kube-proxy in IPVS mode
  * for openstack security groups you have to enable "Other Protocols" for using IPIP (and probably also VxLan)
    * protocol 4
    * protocol 41
  * ipv6 forwarding 
  * ipspoofing in openstack enabled for calico (required)

