# Bolt's Journal - Critical Learnings

## 2026-09-10 - Static HTML performance optimization via Resource Hints and Critical Resource Preloading
**Learning:** In static HTML/CSS web applications relying on third-party CDNs (Bootstrap, Font Awesome, AOS), DNS lookups and TLS handshakes to external domains (`cdn.jsdelivr.net`, `cdnjs.cloudflare.com`) cause layout blocks and network latency. Adding `dns-prefetch` and `preconnect` resource hints optimizes initial connection setup and critical path resource fetching.
**Action:** Always add `dns-prefetch` and `preconnect` links for critical external domains in HTML head sections.
