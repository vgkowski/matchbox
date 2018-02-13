# Matchbox installer

1. Customize `install/dnsmasq.conf` to match the target environment. Specify the mac addresses of your hardware, IPs and hostnames
2. Run `install/matchbox-init <COREOS_CHANNEL> <COREOS_VERSION>` to download CoreOS Container Linux and create matchbox certificates.
 You can customize target directories by overriding `ASSETS_DIR` and `CONFIG_DIR` which defaults to `install/assets` and `install/etc/matchbox`
3. Run `install/matchbox-installer create` to start matchbox and dnsmasq containers
4. Run `install/matchbox-installer status` to get the status of matchbox and dnsmasq
5. Run `install/matchbox-installer destroy` to stop and delete matchbox and dnsmasq containers