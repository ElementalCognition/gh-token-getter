# gha-token-getter

A small application written in Golang built to ease the process of GitHub app token retrieval

Prerequisite:
- Create GitHub application, download private PEM key
- Install GitHub application to your organization
- Pass the following data to the getter
- application id, installation id, location of the private key, name of k8s secret where it will save and update the access token

E.G: 
```bash
gh_get_token -c config_example.yaml
```

Flags:
- "-c", default: "/etc/gh_get_token.conf" - "Token getter config path" 
