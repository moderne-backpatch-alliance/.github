<div align="center">

<img src="https://raw.githubusercontent.com/moderne-backpatch-alliance/.github/main/profile/moderne-icon.svg" alt="Moderne Backpatch Alliance" width="96" height="96">

# Moderne Backpatch Alliance

**Your scanner still flags a patched CVE.**

### [vex.backpatch.moderne.io](https://vex.backpatch.moderne.io)

</div>

---

A backpatch takes the upstream fix for a CVE and applies it to the exact release you
already run, published as `+backpatch.NNN`. It drops in as a binary replacement: the
version and behavior don't change, only the vulnerability is gone.

Because the version number stays the same, your scanner reads it as the old release and
flags the CVE anyway. This feed tells it otherwise. Point Grype, Trivy, JFrog Xray,
Sonatype, or Dependency-Track at the feed and the matching findings clear; each statement
is keyed to an exact package URL.

| Format | Scanners | Feed |
| --- | --- | --- |
| OpenVEX | Grype, Trivy | `https://vex.backpatch.moderne.io/openvex/all.json` |
| CycloneDX | JFrog Xray, Dependency-Track | `https://vex.backpatch.moderne.io/cyclonedx/backpatch-vex.cdx.json` |

See [vex.backpatch.moderne.io](https://vex.backpatch.moderne.io) to configure your scanner or verify a specific fix.

<sub>Maintained by [Moderne](https://www.moderne.io).</sub>
