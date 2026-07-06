<div align="center">

<img src="https://raw.githubusercontent.com/moderne-backpatch-alliance/.github/main/profile/moderne-icon.svg" alt="Moderne Backpatch Alliance" width="96" height="96">

# Moderne Backpatch Alliance

**Your scanner still flags a patched CVE. This is the proof it's already fixed.**

### 🔗 [vex.backpatch.moderne.io](https://vex.backpatch.moderne.io)

</div>

---

A **backpatch** carries the upstream security fix onto the *exact* release you already
run — no major-version jump, no rebuilt artifact, a binary drop-in — published as
`+backpatch.NNN`. Your scanner reads the version number, sees the old release, and flags
the CVE anyway. The VEX feed is the machine-readable proof that it's patched.

Point Grype, Trivy, JFrog Xray, Sonatype, or Dependency-Track at the feed and the matching
CVE findings clear. Every statement matches by exact package URL.

| Format | Scanners | Feed |
| --- | --- | --- |
| **OpenVEX** | Grype · Trivy | `https://vex.backpatch.moderne.io/openvex/all.json` |
| **CycloneDX** | JFrog Xray · Dependency-Track | `https://vex.backpatch.moderne.io/cyclonedx/backpatch-vex.cdx.json` |

**→ Configure your scanner and verify a fix at [vex.backpatch.moderne.io](https://vex.backpatch.moderne.io)**

<sub>Maintained by [Moderne](https://www.moderne.io).</sub>
