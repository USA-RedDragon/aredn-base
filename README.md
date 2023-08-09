# AREDN Virtual Node Base Image

This project is intended to set up a "Cloud Tunnel" for the AREDN network. It acts like a node without any RF link capabilities. The purpose is to allow a large group of users to connect to a tunnel prior to RF deployments being rolled out.

This project requires Linux or WSL2 for the `/dev/net/tun` device

## Updating Patches

This is just a small note to myself documenting the command to update the patches.

`git format-patch --output-directory ../patches/olsrd v0.9.8..HEAD`

Patches sourced from: <https://github.com/aredn/aredn_packages/tree/develop/net/olsrd/patches> and <https://github.com/aredn/aredn_packages/tree/develop/net/vtun/patches>
