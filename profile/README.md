<div align="center">

<img src="https://raw.githubusercontent.com/moderne-backpatch-alliance/.github/main/profile/moderne-icon.svg" alt="Moderne Backpatch Alliance" width="96" height="96">

# Moderne Backpatch Alliance

**Backpatch Alliance is the fellowship of the fix.**

### [backpatch.moderne.io](https://backpatch.moderne.io)

</div>

---

A backpatch applies an upstream security fix to an open source release that no longer
receives fixes, and publishes it under a version derived from that release. A fix for
`2.14.1` ships as `2.14.1.1-backpatch-00001`.

Add the repository to your build, then change the version of the library you are patching.
Anyone can browse the catalog and open any pom. Downloading a backpatch requires an
Alliance membership, which comes with a username and an access token.

The repository is [backpatch.moderne.io/maven/](https://backpatch.moderne.io/maven/) in
Maven layout. The same host also serves npm, PyPI, and NuGet.

Scanners compare versions against advisory ranges, and a backpatch version still falls
inside the range of the release it patches, so they keep reporting a CVE the backpatch
fixed until they read an attestation. Each statement in the feeds names a backpatched
artifact by package URL and says whether a CVE is fixed in it.

| Format | Scanners | Feed |
| --- | --- | --- |
| OpenVEX | Grype, Trivy | `https://backpatch.moderne.io/feeds/openvex/all.json` |
| CycloneDX | JFrog Xray, Sonatype, Dependency-Track | `https://backpatch.moderne.io/feeds/cyclonedx/all.cdx.json` |

See [backpatch.moderne.io/feeds/](https://backpatch.moderne.io/feeds/) to configure a scanner.

<sub>Maintained by [Moderne](https://www.moderne.io).</sub>
