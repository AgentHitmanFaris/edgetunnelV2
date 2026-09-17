# edgetunnel 2.1
![Admin Dashboard](./img.png)

[![Stars](https://img.shields.io/github/stars/cmliu/edgetunnel?style=flat-square&logo=github)](https://github.com/cmliu/edgetunnel/stargazers)
[![Forks](https://img.shields.io/github/forks/cmliu/edgetunnel?style=flat-square&logo=github)](https://github.com/cmliu/edgetunnel/network/members)
[![License](https://img.shields.io/github/license/cmliu/edgetunnel?style=flat-square)](https://github.com/cmliu/edgetunnel/blob/main/LICENSE)
[![Telegram](https://img.shields.io/badge/Telegram-Group-blue?style=flat-square&logo=telegram)](https://t.me/CMLiussss)
[![YouTube](https://img.shields.io/badge/YouTube-Channel-red?style=flat-square&logo=youtube)](https://www.youtube.com/watch?v=LeT4jQUh8ok)
[![zread](https://img.shields.io/badge/Ask_Zread-_.svg?style=flat-square&color=00b0aa&labelColor=000000&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB3aWR0aD0iMTYiIGhlaWdodD0iMTYiIHZpZXdCb3g9IjAgMCAxNiAxNiIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggZD0iTTQuOTYxNTYgMS42MDAxSDIuMjQxNTZDMS44ODgxIDEuNjAwMSAxLjYwMTU2IDEuODg2NjQgMS42MDE1NiAyLjI0MDFWNC45NjAxQzEuNjAxNTYgNS4zMTM1NiAxLjg4ODEgNS42MDAxIDIuMjQxNTYgNS42MDAxSDQuOTYxNTZDNS4zMTUwMiA1LjYwMDEgNS42MDE1NiA1LjMxMzU2IDUuNjAxNTYgNC45NjAxVjIuMjQwMUM1LjYwMTU2IDEuODg2NjQgNS4zMTUwMiAxLjYwMDEgNC45NjE1NiAxLjYwMDFaIiBmaWxsPSIjZmZmIi8%2BCjxwYXRoIGQ9Ik00Ljk2MTU2IDEwLjM5OTlIMi4yNDE1NkMxLjg4ODEgMTAuMzk5OSAxLjYwMTU2IDEwLjY4NjQgMS42MDE1NiAxMS4wMzk5VjEzLjc1OTlDMS42MDE1NiAxNC4xMTM0IDEuODg4MSAxNC4zOTk5IDIuMjQxNTYgMTQuMzk5OUg0Ljk2MTU2QzUuMzE1MDIgMTQuMzk5OSA1LjYwMTU2IDE0LjExMzQgNS42MDE1NiAxMy43NTk5VjExLjAzOTlDNS42MDE1NiAxMC42ODY0IDUuMzE1MDIgMTAuMzk5OSA0Ljk2MTU2IDEwLjM5OTlaIiBmaWxsPSIjZmZmIi8%2BCjxwYXRoIGQ9Ik0xMy43NTg0IDEuNjAwMUgxMS4wMzg0QzEwLjY4NSAxLjYwMDEgMTAuMzk4NCAxLjg4NjY0IDEwLjM5ODQgMi4yNDAxVjQuOTYwMUMxMC4zOTg0IDUuMzEzNTYgMTAuNjg1IDUuNjAwMSAxMS4wMzg0IDUuNjAwMUgxMy43NTg0QzE0LjExMTkgNS42MDAxIDE0LjM5ODQgNS4zMTM1NiAxNC4zOTg0IDQuOTYwMVYyLjI0MDFDMTQuMzk4NCAxLjg4NjY0IDE0LjExMTkgMS42MDAxIDEzLjc1ODQgMS42MDAxWiIgZmlsbD0iI2ZmZiIvPgo8cGF0aCBkPSJNNCAxMkwxMiA0TDQgMTJaIiBmaWxsPSIjZmZmIi8%2BCjxwYXRoIGQ9Ik00IDEyTDEyIDQiIHN0cm9rZT0iI2ZmZiIgc3Ryb2tlLXdpZHRoPSIxLjUiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIvPgo8L3N2Zz4K&logoColor=ffffff)](https://zread.ai/cmliu/edgetunnel)
[![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/cmliu/edgetunnel)

---

## Project Overview

**edgetunnel** is an edge computing tunnel proxy solution built on the Cloudflare Workers / Pages platform. It efficiently handles network traffic while providing a powerful web management console and flexible node configuration options.

- **Demo Site**: [https://EDT-Pages.github.io/admin](https://EDT-Pages.github.io/admin)

### Key Features

- **Protocol Support**: Supports mainstream protocols including VLESS, Trojan, and Shadowsocks with deep integration for encrypted transmission.
- **Management Dashboard**: Built-in visual management panel supporting real-time configuration updates, log viewing, and traffic statistics.
- **Flexible Deployment**: Full compatibility with Cloudflare Workers and Cloudflare Pages (via GitHub repository integration or direct zip upload).
- **Subscription System**: Built-in automatic subscription generation and format conversion, compatible with major clients (Clash, Sing-box, Surge, etc.).
- **Performance Acceleration**: Supports custom ProxyIP, SOCKS5/HTTP chained proxy routing, and optimized node APIs to reduce latency.
- **Cross-Platform Compatibility**: Fully compatible with Windows, Android, iOS, macOS, and various open router / OpenWrt firmware.

---

## Quick Deployment
>[!TIP]
> **Detailed Guide**: [edgetunnel Deployment Guide](https://cmliussss.com/p/edt2/)

>[!WARNING]
> **Error 1101 Issue**: [Video Explanation](https://www.youtube.com/watch?v=r4uVTEJptdE)

### Cloudflare Workers Deployment

<details>
<summary><code><strong>Cloudflare Workers Deployment Guide</strong></code></summary>

1. Deploy CF Worker:
   - In the Cloudflare Workers console, create a new Worker.
   - Paste the code from [_worker.js](https://github.com/cmliu/edgetunnel/blob/main/_worker.js) into the Worker editor.
   - In the left sidebar under Settings, select Variables > Add variable.
     Set the variable name to **ADMIN** and the value to your chosen administrator password, then click Save.

2. Bind KV Namespace:
   - In Settings > Bindings, select Add binding > KV namespace > Add binding, then choose an existing namespace or create a new one.
   - Set the variable name to **KV**, then click Add binding.

3. Bind Custom Domain to Worker:
   - In the Worker console under Triggers, scroll down and click Add Custom Domain.
   - Enter a subdomain that is managed by Cloudflare DNS (e.g. `vless.yourdomain.com`), click Add Custom Domain, and wait for the SSL certificate to activate.

4. Access Dashboard:
   - Visit `https://vless.yourdomain.com/admin` and log in with your administrator password.

</details>

### Cloudflare Pages Direct Upload Deployment (Recommended) - [Visual Guide](https://cmliussss.com/p/edt2/)

<details>
<summary><code><strong>Pages Direct Upload Deployment Guide</strong></code></summary>

1. Deploy CF Pages:
   - Download the repository archive [main.zip](https://github.com/cmliu/edgetunnel/archive/refs/heads/main.zip), and star this repository.
   - In the Cloudflare Pages console, choose Upload assets, name your project, click Create project, upload the downloaded [main.zip](https://github.com/cmliu/edgetunnel/archive/refs/heads/main.zip) archive, and click Deploy site.
   - After deployment completes, click Continue to project, then navigate to Settings > Environment variables > Production > Add variable.
     Set the variable name to **ADMIN** and the value to your chosen administrator password, then click Save.
   - Go back to the Deployments tab, click Create new deployment on the right, re-upload [main.zip](https://github.com/cmliu/edgetunnel/archive/refs/heads/main.zip), and click Save and Deploy.

2. Bind KV Namespace:
   - In Settings > Bindings, select Add > KV namespace, then select an existing namespace or create a new one.
   - Set the variable name to **KV**, then click Save and re-deploy.

3. Bind CNAME Custom Domain to Pages: [Video Tutorial](https://www.youtube.com/watch?v=LeT4jQUh8ok&t=851s)
   - In the Pages console under Custom domains, click Set up a custom domain.
   - Enter your custom subdomain (do not use your apex root domain; for example, if your domain is `example.com`, enter `node.example.com`).
   - In your DNS provider, create a CNAME record for that subdomain pointing to `<your-project>.pages.dev` as instructed by Cloudflare, then click Activate domain.

4. Access Dashboard:
   - Visit `https://node.example.com/admin` and log in with your administrator password.

</details>

### Cloudflare Pages + GitHub Deployment

<details>
<summary><code><strong>Pages + GitHub Deployment Guide</strong></code></summary>

1. Deploy CF Pages:
   - Fork this repository on GitHub and star it.
   - In the Cloudflare Pages console, choose Connect to Git, select your fork of `edgetunnel`, and click Begin setup.
   - In the Build and deployment settings page, expand Environment variables (advanced) and click Add variable.
     Set the variable name to **ADMIN** and the value to your chosen administrator password, then click Save and Deploy.

2. Bind KV Namespace:
   - In Settings > Bindings, select Add > KV namespace, then choose an existing namespace or create a new one.
   - Set the variable name to **KV**, then click Save and re-deploy.

3. Bind CNAME Custom Domain to Pages: [Video Tutorial](https://www.youtube.com/watch?v=LeT4jQUh8ok&t=851s)
   - In the Pages console under Custom domains, click Set up a custom domain.
   - Enter your custom subdomain (e.g. `node.example.com`).
   - In your DNS provider, create a CNAME record pointing to `<your-project>.pages.dev`, then click Activate domain.

4. Access Dashboard:
   - Visit `https://node.example.com/admin` and log in with your administrator password.

</details>

---

## Environment Variables

| Variable | Required | Example | Description |
| :--- | :---: | :--- | :--- |
| **ADMIN** | Yes | `123456` | Password to access the admin web dashboard. |
| **KEY** | No | `CMLiussss` | Quick subscription secret path. Accessing `/<KEY>` immediately returns node subscriptions. |
| **UUID** | No | `90cd4a77-141a-43c9-991b-08263cfe9c10` | Enforces a fixed UUID. Must be in valid **UUIDv4** standard format. |
| **PROXYIP** | No | `proxyip.cmliussss.net:443` | Global custom reverse proxy IP and port. |
| **URL** | No | `https://cloudflare-error-page-3th.pages.dev` | Default homepage disguise URL (can be a website URL or `1101`). |
| **GO2SOCKS5** | No | `blog.cmliussss.com,*.ip111.cn,*google.com` | Domains forced to route through SOCKS5 (`*` for global routing, comma-separated). |
| **DEBUG** | No | `1` or `true` | Developer mode. Debug logging (`console.log`) is disabled by default. Set to `1` or `true` to enable. |
| **OFF_LOG** | No | `1` or `true` | KV access logging is enabled by default. Set to `1` or `true` to disable logging. |
| **BEST_SUB** | No | `1` or `true` | Best node subscription generator feature. Disabled by default. Set to `1` or `true` to enable. |
| **PRELOAD_RACE_DIAL** | No | `1` or `true` | TCP preload race dialing. Disabled by default. Set to `1` or `true` to enable. |
| **TCP_CONCURRENT_DIAL** | No | `2` | Number of concurrent TCP dialing attempts (default: `2`). When configured, does not downgrade automatically to single-route on China Mobile networks. |
| **PROXY_CONCURRENT_DIAL** | No | `1` | Number of concurrent reverse proxy dialing attempts (default: `1`). Higher values connect faster but rotate IPs more frequently. |

---

## Advanced Usage & Tips

To modify the subscription TOKEN and node validation UUID:
1. Modifying the `ADMIN` or `KEY` variable will automatically change the subscription TOKEN and validation UUID.
2. Setting the `UUID` variable enforces a fixed subscription TOKEN and validation UUID. Note: It must strictly follow the **UUIDv4** standard format, otherwise nodes will fail to connect.

This project supports dynamically switching the proxy backend via URL path:

- Specify `PROXYIP` example:
  ```url
  /proxyip=proxyip.cmliussss.net
  /?proxyip=proxyip.cmliussss.net
  ```

- Specify `SOCKS5` example:
  ```url
  /socks5=user:password@127.0.0.1:1080
  /?socks5=user:password@127.0.0.1:1080
  /socks://dXNlcjpwYXNzd29yZA==@127.0.0.1:1080 (activates global SOCKS5 by default)
  /socks5://user:password@127.0.0.1:1080 (activates global SOCKS5 by default)
  ```

- Specify `HTTP Proxy` example:
  ```url
  /http=user:password@127.0.0.1:1080
  /http://user:password@127.0.0.1:8080 (activates global SOCKS5 by default)
  ```

- Specify `Trojan Fallback` example:
  (Intended for self-hosted setups: Trojan inbound only; fallback service must use the same password, non-WebSocket, non-TLS. UDP is passed directly to fallback for high performance and compatibility):
  ```url
  /trojan=1.1.1.1:1234
  ```

---

## Supported Clients

| Platform | Recommended Clients |
| :--- | :--- |
| **Windows** | [v2rayN](https://github.com/2dust/v2rayN/releases), [Hiddify](https://github.com/hiddify/hiddify-app/releases), [FlClash](https://github.com/chen08209/FlClash/releases), [mihomo-party](https://github.com/mihomo-party-org/clash-party/releases), [Clash Verge Rev](https://github.com/clash-verge-rev/clash-verge-rev/releases), [Clashmi](https://github.com/KaringX/clashmi/releases), [FlyClash](https://github.com/GtxFury/FlyClash/releases), [Karing](https://github.com/KaringX/karing/releases), [Bettbox](https://github.com/appshubcc/Bettbox/releases) |
| **Android** | [v2rayNG](https://github.com/2dust/v2rayNG/releases), [ClashMetaForAndroid](https://github.com/MetaCubeX/ClashMetaForAndroid/releases/), [FlClash](https://github.com/chen08209/FlClash/releases), [Clashmi](https://github.com/KaringX/clashmi/releases), [Hiddify](https://github.com/hiddify/hiddify-app/releases), [NekoBox](https://github.com/MatsuriDayo/NekoBoxForAndroid/releases), [FlyClash](https://github.com/GtxFury/FlyClash/releases), [Karing](https://github.com/KaringX/karing/releases), [Bettbox](https://github.com/appshubcc/Bettbox/releases) |
| **iOS** | Surge, Shadowrocket, Stash, [Hiddify](https://github.com/hiddify/hiddify-app/releases), Loon, Egern, [Clashmi](https://clashmi.app/download), [Karing](https://karing.app/), Quantumult X |
| **macOS** | [FlClash](https://github.com/chen08209/FlClash/releases), [mihomo-party](https://github.com/mihomo-party-org/clash-party/releases), [Clash Verge Rev](https://github.com/clash-verge-rev/clash-verge-rev/releases), Surge, [Clashmi](https://clashmi.app/download), [Karing](https://karing.app/), [FlyClash](https://github.com/GtxFury/FlyClash/releases) |
| **HarmonyOS** | [ClashBox](https://github.com/xiaobaigroup/ClashBox/releases) |

---

## Project Popularity

![Stargazers over time](https://github.com/cmliu/cmliu/blob/main/star/edgetunnel.svg)

---

## Acknowledgments & Credits

### Sponsorship Support - Providing Cloud Servers to Maintain the Subscription Conversion Service
- [Yuusei Network](https://yuusei.io/)
- [VMRack](https://www.vmrack.net?ref_code=5Zk7eNhbgL7)

### Open Source References
- [zizifn/edgetunnel](https://github.com/zizifn/edgetunnel)
- [3Kmfi6HP/EDtunnel](https://github.com/6Kmfi6HP/EDtunnel)
- [SHIJS1999/cloudflare-worker-vless-ip](https://github.com/SHIJS1999/cloudflare-worker-vless-ip)
- [Stanley-baby](https://github.com/Stanley-baby)
- [ACL4SSR](https://github.com/ACL4SSR/ACL4SSR/tree/master/Clash/config)
- [CF_NAT](https://t.me/CF_NAT/38889)
- [Workers/Pages Metrics](https://t.me/zhetengsha/3382)
- [bestcfipas](https://t.me/bestcfipas)
- [Mingyu](https://github.com/ymyuuu/workers-vless)
- [ToiCF/CF-Workers-HTTPS](https://github.com/ToiCF/CF-Workers-HTTPS)
- [ToiCF/CF-Workers-TURN](https://github.com/ToiCF/CF-Workers-TURN)
- [ToiCF/CF-Workers-SoftEther](https://github.com/ToiCF/CF-Workers-SoftEther)
- [eooce](https://github.com/eooce/Cloudflare-proxy)
- [Sukka](https://ip.skk.moe/)
- [zhangtaile](https://github.com/cmliu/edgetunnel/pull/999)
- [1345695](https://github.com/1345695/edcloudwasm)
- [ToiCF/GrainTCP](https://github.com/ToiCF/GrainTCP)
- [xream](https://github.com/cmliu/edgetunnel/pull/1359)

---

## Disclaimer

1. This project ("edgetunnel") is intended strictly for educational, research, and personal security testing purposes.
2. Users must comply with all applicable local laws and regulations when using or downloading this code.
3. The author assumes no liability or responsibility for any actions or consequences resulting from the misuse of this project.
4. This project is provided as-is without warranty; no liability is accepted for direct or indirect damages arising from its use.
5. It is recommended to delete any test deployments within 24 hours after evaluation.

---

**If you find this project useful, please star the repository!**
