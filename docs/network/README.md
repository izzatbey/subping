<!-- Code generated by gomarkdoc. DO NOT EDIT -->

# network

```go
import "github.com/fadhilyori/subping/pkg/network"
```

## Index

- [func FindIPsOutsideSubnet\(ipAddresses \[\]net.IP, subnet \*net.IPNet\) \[\]net.IP](<#FindIPsOutsideSubnet>)
- [func GenerateIPListFromCIDR\(firstIp net.IP, cidr \*net.IPNet\) \[\]net.IP](<#GenerateIPListFromCIDR>)
- [func GenerateIPListFromCIDRString\(cidr string\) \(\[\]net.IP, error\)](<#GenerateIPListFromCIDRString>)


<a name="FindIPsOutsideSubnet"></a>
## func FindIPsOutsideSubnet

```go
func FindIPsOutsideSubnet(ipAddresses []net.IP, subnet *net.IPNet) []net.IP
```

FindIPsOutsideSubnet returns a list of IP addresses from the given slice that are outside the specified subnet.

<a name="GenerateIPListFromCIDR"></a>
## func GenerateIPListFromCIDR

```go
func GenerateIPListFromCIDR(firstIp net.IP, cidr *net.IPNet) []net.IP
```

GenerateIPListFromCIDR generates a list of IP addresses within the specified range based on the given IP and CIDR notation.

<a name="GenerateIPListFromCIDRString"></a>
## func GenerateIPListFromCIDRString

```go
func GenerateIPListFromCIDRString(cidr string) ([]net.IP, error)
```

GenerateIPListFromCIDRString parses the given CIDR string and generates a list of IP addresses within the specified range. The CIDR string should be in the form "ip/mask", e.g., "192.168.0.0/24".

Generated by [gomarkdoc](<https://github.com/princjef/gomarkdoc>)