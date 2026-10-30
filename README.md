# Cantarella Solver - Cloudflare Turnstile Solver, IUAM & Challenge Bypass API

[![Website](https://img.shields.io/badge/Website-cantarellasolver.me-0ea5e9?style=for-the-badge)](https://cantarellasolver.me)
[![Telegram](https://img.shields.io/badge/Telegram-@cantarellasolves-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/cantarellasolves)
[![Pass Rate](https://img.shields.io/badge/Pass%20Rate-99.1%25%20Verified-22c55e?style=for-the-badge)](https://cantarellasolver.me)
[![Average Speed](https://img.shields.io/badge/Avg%20Speed-1--3s-orange?style=for-the-badge)](https://cantarellasolver.me)
[![Architecture](https://img.shields.io/badge/Engine-Bare--Metal%20Rust-red?style=for-the-badge)](https://cantarellasolver.me)

> **The fastest, lowest-cost Cloudflare Turnstile Solver & IUAM (Under Attack Mode) Bypass API.**  
> Built for web scrapers, automation bots, and data pipelines in Python, Node.js, Go, and cURL. Get valid Turnstile tokens and `cf_clearance` cookies in **1–3 seconds** with **99.1%+ verified pass rate**.

| Requests Processed | Verified Pass Rate | Average Solve Time | PAYGO Starting Rate |
| :----------------: | :----------------: | :----------------: | :-----------------: |
| **500M+** | **99.1%** | **< 3s** | **$0.08 / 1k** |

> **Failed solves are never billed.** Only pay for verified, valid tokens and clearances.  
> 🎁 **Welcome Bonus:** 1,250 free solves ($0.10 starter credit) automatically added upon signup.

---

## 🔍 Why Cantarella is the #1 Turnstile & IUAM Solver

- ⚡ **Ultra-Fast Turnstile Solver:** Average solve speed of **1.2s – 2.8s** (3x faster than CapSolver or 2Captcha).
- 🛡️ **Complete IUAM / IAUM Solver:** Bypass Cloudflare's "I'm Under Attack Mode" and 5-second challenge screens to generate clean `cf_clearance` cookies.
- 🚀 **100% Browserless & Headless:** Native Rust VM emulation without heavy Chromium, Puppeteer, or Playwright memory overhead.
- 💸 **Unbeatable Pricing:** Starting at just **$0.08 per 1,000 solves** ($0.00008/solve). Failed challenges and timeouts are 100% free.
- 📈 **Extreme Concurrency:** Seamlessly handle up to **18,000+ CPM (Challenges Per Minute)** with dedicated worker pools.
- 🌐 **Proxy Optional:** Solve Turnstile directly with zero proxy requirements, or pass your own HTTP/HTTPS/SOCKS5 residential proxies.
- 🔄 **Drop-in CapSolver / 2Captcha Migration:** Swap your base URL and API key in 60 seconds.

---

## 💰 Pricing & Plans

We offer two transparent pricing models: **Pay-As-You-Go** for flexible on-demand volume, and **Unlimited Concurrency Plans** for high-volume 24/7 scraping with zero per-request fees.

### 1. Pay-As-You-Go (PAYGO)

Pay strictly for successful solves. No monthly commitments, no maintenance fees.

* **Rate per single solve:** **$0.00008**
* **Rate per 1,000 solves:** **$0.08**
* **Welcome Credit:** 1,250 free solves ($0.10 starter balance)

#### 🧮 PAYGO Cost Breakdown

| Challenge Solves | Calculation | Total Cost |
| :--- | :--- | :--- |
| **1,000 solves** | 1,000 × $0.00008 | **$0.08** |
| **5,000 solves** | 5,000 × $0.00008 | **$0.40** |
| **10,000 solves** | 10,000 × $0.00008 | **$0.80** |
| **25,000 solves** | 25,000 × $0.00008 | **$2.00** |
| **50,000 solves** | 50,000 × $0.00008 | **$4.00** |
| **100,000 solves** | 100,000 × $0.00008 | **$8.00** |
| **500,000 solves** | 500,000 × $0.00008 | **$40.00** |
| **1,000,000 solves** | 1,000,000 × $0.00008 | **$80.00** |

$$\text{Total Cost} = \text{Solves} \times \$0.00008$$

---

### 2. Ready-Made Unlimited Concurrency Plans

Unlimited plans reserve a dedicated parallel thread pool with **zero per-request fees**. Solve 24/7 with unlimited challenges without counting requests.

| Plan | Threads | Max Throughput | Daily (24h) | Weekly (7d) | Monthly (30d) | Best For |
| :--- | :---: | :---: | :---: | :---: | :---: | :--- |
| **Core** | **100** | ~1,800 / min | **$4.25** | **$18.50** | **$54.00** | Moderate scrapers & steady production traffic |
| **Growth** | **200** | ~3,600 / min | **$8.50** | **$36.00** | **$99.00** | Parallel scrapers & background pipelines |
| **Scale** | **500** | ~9,000 / min | **$21.50** | **$89.00** | **$249.00** | High-volume crawling clusters |
| **Unlimited** ⭐ | **1,000** | ~18,000 / min | **$42.50** | **$169.00** | **$429.00** | Enterprise scraping at maximum solver capacity |

* **Max Speed Estimate:** $\text{Threads} \times 18 = \text{Estimated Challenges Per Minute (CPM)}$
* **All plans include:** Auto load-balancing across multi-node cluster, sub-3 second solve times, and Turnstile + IUAM compatibility.

---

### 3. Custom Thread Pool Rate Calculator

Need a specific thread count (e.g. 50, 150, 300, or 750 threads)? Custom thread pools scale linearly with no markup:

| Duration | Rate Per Thread | Formula | Example (250 Threads) |
| :--- | :---: | :--- | :--- |
| **Daily** (24 hrs) | **$0.0425** / thread | $\text{Threads} \times \$0.0425$ | $250 \times \$0.0425 =$ **$10.63** |
| **Weekly** (7 days) | **$0.1850** / thread | $\text{Threads} \times \$0.1850$ | $250 \times \$0.1850 =$ **$46.25** |
| **Monthly** (30 days) | **$0.5400** / thread | $\text{Threads} \times \$0.5400$ | $250 \times \$0.5400 =$ **$135.00** |

---

## 🔄 Drop-in Migration

Coming from CapSolver, 2Captcha, Anti-Captcha, Solverify, NSLSolver, CapMonster, NextCaptcha, EzCaptcha, or NopeCHA? Migration takes less than 60 seconds:

1. **Base URL** → `https://cantarellasolver.me`
2. **API Key Header** → Pass your Wuwa API key via `Wuwa-Api-Key`

---

## ⚡ Quick Start & Code Examples

All requests use the standard API endpoint and authorization header:

```http
POST https://cantarellasolver.me/task
Wuwa-Api-Key: YOUR_API_KEY
Content-Type: application/json
```

### 1. Cloudflare Turnstile Solver (Python)

Solve Turnstile managed, non-interactive, or invisible challenge widgets:

```python
import requests

response = requests.post(
    "https://cantarellasolver.me/task",
    headers={"Wuwa-Api-Key": "YOUR_API_KEY"},
    json={
        "mode": "turnstile",
        "url": "https://target-website.com/login",
        "sitekey": "0x4AAAAAAAA1WzHSsbGWTH88",
    },
    timeout=30
)

print(response.json())
```

**Success Response (HTTP 200)**

```json
{
  "token": "0.3g00PIzENb3goEq4-D.....",
  "elapsed": "1.42s",
  "status": "completed"
}
```

| Field | Required | Description |
| ----- | :------: | ----------- |
| `mode` | Yes | Must be `turnstile` |
| `url` | Yes | Target URL hosting the Cloudflare Turnstile widget |
| `sitekey` | Yes | Turnstile public sitekey (`0x4AAAAAAAA...`) |
| `action` | No | Optional: Widget `action` parameter (e.g. `login`), if specified by target |
| `cdata` | No | Optional: Custom `cData` string, if specified by target |
| `proxy` | No | Optional: Proxy in `http://`, `https://`, or `socks5://` format |

---

### 2. Cloudflare IUAM / IAUM Solver (Python)

Bypass Cloudflare Under Attack Mode and extract a valid `cf_clearance` cookie:

```python
import requests

response = requests.post(
    "https://cantarellasolver.me/task",
    headers={"Wuwa-Api-Key": "YOUR_API_KEY"},
    json={
        "mode": "iuam",
        "url": "https://target-website.com/",
        # "proxy": "socks5://user:pass@host:port"  # Optional
    },
    timeout=35
)

print(response.json())
```

**Success Response (HTTP 200)**

```json
{
  "headers": {
    "Cookie": "cf_clearance=cZ3ow5J194Lyer0BTI64.....;",
    "User-Agent": "Mozilla/5.0 (iPhone; CPU iPhone OS 17_0 like Mac OS X)..."
  },
  "ip": "104.28.x.x",
  "elapsed": "2.10s",
  "status": "completed"
}
```

> **Tip:** If you provide an optional proxy, replay the returned `Cookie` and `User-Agent` through the same proxy for seamless session continuity.

| Field | Required | Description |
| ----- | :------: | ----------- |
| `mode` | Yes | Must be `iuam` |
| `url` | Yes | Target protected challenge page URL |
| `proxy` | No | Optional: `http://`, `https://`, or `socks5://` proxy |

---

### 3. cURL Example

```bash
curl -X POST https://cantarellasolver.me/task \
  -H "Wuwa-Api-Key: YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "mode": "turnstile",
    "url": "https://target-website.com/login",
    "sitekey": "0x4AAAAAAAA1WzHSsbGWTH88"
  }'
```

---

### 4. Node.js / TypeScript Example

```typescript
const response = await fetch("https://cantarellasolver.me/task", {
  method: "POST",
  headers: {
    "Wuwa-Api-Key": "YOUR_API_KEY",
    "Content-Type": "application/json"
  },
  body: JSON.stringify({
    mode: "turnstile",
    url: "https://target-website.com/login",
    sitekey: "0x4AAAAAAAA1WzHSsbGWTH88"
  })
});

const data = await response.json();
console.log("Turnstile Token:", data.token);
```

---

### Errors & Failed Solves

Failed solves or timeouts return a standard failure payload and are **never billed**:

```json
{
  "message": "Challenge solve failed or timed out",
  "status": "failed"
}
```

---

## 🎯 Frequently Searched Queries & Solutions

<details>
<summary><b>How to solve Cloudflare Turnstile in Python?</b></summary>

Use Cantarella Solver's REST API. Send a POST request to `https://cantarellasolver.me/task` with `mode: "turnstile"`, target page `url`, and the Turnstile `sitekey`. In under 2 seconds, you receive the `token` string which you can inject directly into your form's `cf-turnstile-response` input.
</details>

<details>
<summary><b>How to bypass Cloudflare IUAM (Under Attack Mode) 5-second challenge?</b></summary>

Send a request with `mode: "iuam"` and the target URL. Cantarella Solver navigates the challenge via native Rust VM emulation and returns the valid `cf_clearance` cookie and matching `User-Agent` to pass directly to your HTTP client.
</details>

<details>
<summary><b>Is Cantarella Solver faster than CapSolver or 2Captcha?</b></summary>

Yes. Most traditional services rely on slow browser automation (taking 12–25 seconds) or human clickers. Cantarella executes Cloudflare challenge bytecode directly inside a high-speed, native Rust engine in **1.2 to 2.8 seconds** with a 99.1%+ pass rate.
</details>

---

## 🤝 Support & Community

Join our official channels for real-time announcements, uptime monitoring, and API support:

| Channel | Link |
| :--- | :--- |
| **Website & Dashboard** | [cantarellasolver.me](https://cantarellasolver.me) |
| **Telegram Updates & Support** | [@cantarellasolves](https://t.me/cantarellasolves) |
| **Direct Contact** | [t.me/cantarellasolves](https://t.me/cantarellasolves) |

---

© 2026 Cantarella Solver. High-speed, bare-metal Turnstile & IUAM challenge resolution.
