# Install x00.sh Root CA

## Linux // Ubuntu
Ensure you have the ca-certificates utility installed.

```bash
apt-get install ca-certificates
```

Fetch CA.crt

```bash
curl -L https://raw.githubusercontent.com/x00-sh/ca/main/ca.crt | sudo tee /usr/share/ca-certificates/x00-sh-ca.crt && sudo dpkg-reconfigure ca-certificates
```

Make sure you tick off x00-sh-cz.crt. Press OK.

## Linux // Fedora
```
curl -L https://raw.githubusercontent.com/x00-sh/ca/main/ca.crt | sudo tee /etc/pki/ca-trust/source/anchors/x00-sh-ca.crt && sudo update-ca-trust
```

## Windows

Download [https://raw.githubusercontent.com/x00-sh/ca/main/ca.p12] and install into the `Trusted Root Certification Authorities` store.
