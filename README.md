### Ali Ganiyev — Security Researcher

Independent security researcher focused on vulnerability discovery and patch development in
software — threat-intelligence platforms, offensive-security tooling, and the Linux
kernel. Every item below is upstream-verified: a merged patch, a vendor advisory, or both.

---

#### CVEs

| CVE | Project | Vulnerability | Fixed in |
|---|---|---|---|
| [CVE-2026-121139](https://www.cve.org/CVERecord?id=CVE-2026-121139) | Rapid7 **Metasploit Framework** | Missing authentication in the `msf-ws` REST API (CWE-306). A bootstrap exemption in `ApiToken#authenticate!` returned success whenever `msf.auth_initialized` was false, short-circuiting the `AdminApiToken` check — so an unauthenticated caller could `POST /api/v1/users` and create the first **administrator**. CVSS 3.1 **7.8 High**. | [6.5.9](https://github.com/rapid7/metasploit-framework/pull/22039) |
| [CVE-2026-9084](https://nvd.nist.gov/vuln/detail/CVE-2026-9084) | **MISP** | OIDC authentication bypass under insecure IdP configurations, allowing account takeover via **email claim spoofing**. Credited as discoverer. | [PR #10784](https://github.com/MISP/MISP/pull/10784) |

> CVE-2026-121139 was reported independently by two researchers; credit is shared.

#### Upstream patches and credited reports

- **Linux Kernel (stable 6.6.144)** — `ksmbd: OOB read regression in smb_check_perm_dacl() ACE-walk loops`
  Fixed an out-of-bounds read regression in the kernel SMB server (ksmbd).
  [Patch — lore.kernel.org](https://lore.kernel.org/stable/)
  `Signed-off-by: Ali Ganiyev <ali.qaniyev@gmail.com>`

- **TheHive Project / Cortex-Analyzers** — [PR #1456](https://github.com/TheHive-Project/Cortex-Analyzers/pull/1456): EmlParser security hardening (safe attachment filenames, removed insecure `umask`/world-writable directory creation). Credited as discoverer.

- **TheHive Project / Cortex-Analyzers** — [PR #1457](https://github.com/TheHive-Project/Cortex-Analyzers/pull/1457): UnshortenLink SSRF host-filter hardening, follow-up to CVE-2019-7652. Credited as discoverer.

---

**Projects:**

- [Researcher](https://github.com/aliganiyev/Researcher) — this portfolio, in detail

<sub>Research above is conducted and disclosed in a personal capacity.</sub>
