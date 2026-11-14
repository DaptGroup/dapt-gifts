# Dapt gifts

Free SharePoint web parts from [Dapt](https://www.daptgroup.com). Download the package, upload it to your App Catalog and add it to a page. No licence key, no Azure and no admin API approvals.

| Gift | What it does | Download |
| --- | --- | --- |
| [**Dapt Copilot Advent**](copilot-advent/) | A Copilot tip advent calendar. Try a prompt each day, tick the door off and help get Santa's sleigh ready for Christmas. | [Latest release](https://github.com/DaptGroup/dapt-gifts/releases?q=copilot-advent) |
| [**Dapt Site Assessment**](site-assessment/) | A health check for a SharePoint site: redundant, obsolete and trivial content, structure, metadata and permissions, with a score from A to E and a PDF report. | [Latest release](https://github.com/DaptGroup/dapt-gifts/releases?q=site-assessment) |

## Getting a package

1. Open **[Releases](https://github.com/DaptGroup/dapt-gifts/releases)** and choose the newest release of the gift you want.
2. Download the `.sppkg` file under **Assets**.
3. Optional: check the file against the SHA-256 checksum in the release notes. In PowerShell, run `Get-FileHash .\dapt-advent.sppkg`.
4. Follow the install guide in the gift's folder.

Packages are only published as release assets. They are never committed to the repository.

## What you need

- SharePoint Online (Microsoft 365).
- Someone who can upload apps to the tenant App Catalog (SharePoint Administrator or Global Administrator), or a site collection App Catalog.
- A modern SharePoint page to add the web part to.

## Good to know

- These are free, ready-built packages. The source code is not published here.
- Each package is a SharePoint Framework (SPFx 1.21) solution built and signed off by Dapt UK Ltd.
- Questions, problems or ideas: [open an issue](https://github.com/DaptGroup/dapt-gifts/issues) or email hello@daptgroup.com.
- Found a security problem? Please see [SECURITY.md](SECURITY.md) and don't post it as a public issue.

## Want more?

Dapt builds Microsoft 365 solutions on four lines: **B**uild (Dapt Webparts), **A**dvise (Dapt Consult), **G**overn (Orchestry) and **S**upport. [Talk to Dapt](https://www.daptgroup.com).

See [LICENSE.md](LICENSE.md) for the terms of use. © Dapt UK Ltd.
