# Jadarit

A self-hosted live media server. RTMP and WebRTC in, HLS and sub-second WebRTC
out, server-side ad insertion and adaptive bitrate. One binary on your own
hardware, with no per-viewer fees.

This repository publishes the official builds. Documentation, pricing and
licences are at **[jadarit.com](https://jadarit.com)**.

## Install

### Debian and Ubuntu

```bash
curl -LO https://github.com/Jadarit-com/jadarit-releases/releases/latest/download/jadarit_amd64.deb
curl -LO https://github.com/Jadarit-com/jadarit-releases/releases/latest/download/SHA256SUMS
sha256sum -c --ignore-missing SHA256SUMS
sudo apt install ./jadarit_amd64.deb
```

The checksum step confirms the package arrived complete and is exactly the
file published here.

### Container

```bash
docker pull ghcr.io/jadarit-com/jadarit:latest
```

The [install guide](https://jadarit.com/docs/start/install/) covers ports,
volumes and the first sign-in for both.

## Licence

Every install runs a free 30-day trial with all features. To keep using it, buy
a licence at [jadarit.com](https://jadarit.com/#pricing); it is emailed to you
and installs with `sudo jadarit license install <file>`.

## Help

- **Something not working?** [Open a bug report](https://github.com/Jadarit-com/jadarit-releases/issues/new/choose).
  Running `jadarit doctor` first often explains it.
- **Licences, invoices and sales:** [jadarit.com/contact](https://jadarit.com/contact/)
- **Security issues:** please report privately, see [SECURITY.md](SECURITY.md).
