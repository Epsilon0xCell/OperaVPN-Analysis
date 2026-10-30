![OperaVPN-Analysis](banner.png)

# OperaVPN-Analysis

An investigative report on the Opera GX browser's built-in "free VPN": what it actually does technically, whether it leaks data, how Opera's logging claims have changed, and what Opera's corporate ownership means for trust.

## The report

- [Opera GX VPN: Trustworthy?](Opera-GX-VPN-Trustworthy.pdf) - the full report as a PDF (21 pages, exported from Google Docs).

## What it covers

1. **Technical architecture** - The free service is a browser-only HTTPS proxy, not a system-wide VPN: it protects only traffic inside the Opera browser and uses no tunneling protocol such as OpenVPN or WireGuard. The paid VPN Pro tier, by contrast, is a genuine system-wide VPN (Lightway, OpenVPN, IKEv2, kill switch, 3,000+ servers), and the report argues the free tier's limits function as an upsell funnel.
2. **Data integrity** - WebRTC and DNS leak exposure in the free service, and the manual settings changes a user must make to mitigate them, which sits awkwardly next to the product's "zero extra steps" marketing.
3. **Logging policy** - Historical logging allegations contrasted with Opera's current no-log claims and the September 2024 Deloitte audit.
4. **Corporate ownership** - Opera's 2016 acquisition by a Chinese consortium led by Kunlun Tech, the CFIUS-ordered Grindr divestiture as a precedent, and China's National Intelligence Law, weighed against Opera's Norwegian jurisdiction and GDPR defense.
5. **Final verdict and recommendations** - acceptable and dangerous use cases by risk profile.

## Verdict, in short

- On effectiveness: **No.** The free service is not an effective tool for comprehensive data protection. It is acceptable only for casual IP masking, simple geo-restriction bypassing, and light encryption on public Wi-Fi, and it is dangerous for torrenting, sensitive activity, or protection against targeted adversaries.
- On trustworthiness: **Yes, too shaky for privacy-first users.** The ownership structure creates a risk that no technical audit can retire, even though the current no-log configuration was independently audited.

## Scope and limits

This repository contains the finished report only; there is no code and nothing to run. The report's findings are its author's synthesis of the 49 sources in its reference list (accessed 8 July 2025, per the report). Those sources were not independently re-verified for this README; the section summaries and verdicts above are taken directly from the report's own text.
