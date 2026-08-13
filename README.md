### Ali Ganiyev — Security Researcher

Independent security researcher focused on vulnerability discovery and patch development in open-source software.

**Verified contributions:**

- **Linux Kernel (stable 6.6.144)** — `ksmbd: OOB read regression in smb_check_perm_dacl() ACE-walk loops`
  Fixed an out-of-bounds read regression in the kernel SMB server (ksmbd).
  [Patch — lore.kernel.org](https://lore.kernel.org/stable/)
  `Signed-off-by: Ali Ganiyev <ali.qaniyev@gmail.com>`

- **TheHive Project / Cortex-Analyzers** — [PR #1456](https://github.com/TheHive-Project/Cortex-Analyzers/pull/1456): EmlParser security hardening (safe attachment filenames, removed insecure `umask`/world-writable directory creation). Credited as discoverer.

- **TheHive Project / Cortex-Analyzers** — [PR #1457](https://github.com/TheHive-Project/Cortex-Analyzers/pull/1457): UnshortenLink SSRF host-filter hardening, follow-up to CVE-2019-7652. Credited as discoverer.

- **MISP** — [CVE-2026-9084](https://nvd.nist.gov/vuln/detail/CVE-2026-9084) / [PR #10784](https://github.com/MISP/MISP/pull/10784): OIDC authentication bypass under insecure IdP configurations, allowing account takeover via email claim spoofing. Credited as discoverer.

**Projects:**

- [Researcher](https://github.com/aliganiyev/Researcher) — this portfolio, in detail
