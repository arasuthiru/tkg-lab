
### Deploy External DNS
Below script installs External DNS.

## AWS

```bash
./shared-cluster-setup/aws/scripts/03a-install-external-dns.sh
```

## vSphere

#### Install Metallb first

Make sure to change ip ranges according to your env. 
./shared-services-cluster-setup/vsphere/lib/metallb_values.yaml 

```bash
./shared-cluster-setup/vsphere/scripts/03-install-metallb.sh
```
#### Install External DNS

```bash
./shared-cluster-setup/vsphere/scripts/04a-install-external-dns.sh
```
Continue to Next Step: [Configure Contour](04_configure_contour.md)
