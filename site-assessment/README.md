# Dapt Site Assessment (free edition)

A health check for a SharePoint site. It finds redundant, obsolete and trivial (ROT) content, structure problems, metadata gaps and permissions worth a look, then gives the site a score out of 100 and a grade from A to E. You also get a Dapt-branded PDF report.

**Package:** `dapt-site-assessment.sppkg` · **Current version:** 1.2.0 · [Download from Releases](https://github.com/DaptGroup/dapt-gifts/releases?q=site-assessment)

The release also includes three PDF guides: the user guide, the install and admin guide, and the security and privacy summary.

## What it checks

| Area | Examples |
| --- | --- |
| Redundant | Duplicate copies, "Copy of" and "final_v2" files, files with 100 or more versions |
| Obsolete | Files not changed in years, files never opened, libraries nobody uses |
| Trivial | Empty files and folders, lock, temp and backup files |
| Structure | Deep folders, paths near SharePoint's limits, very large folders, big libraries with no indexes, version settings |
| Metadata | Libraries with no columns of their own, or with columns mostly left blank |
| Access | Files, folders and libraries with their own permissions, checked-out files |

The score is built from Clean (25%), Fresh (20%), Structure (20%), Metadata (20%) and Access (15%). You also get an outline of what a better structure could look like.

## Free edition

The free edition shows **what** needs attention. Fixing it is where Dapt can help.

| | Free (this package) | Dapt Site Assessment Pro |
| --- | --- | --- |
| Score, grade, charts and all headline numbers | ✓ | ✓ |
| Rows listed per finding | 5 examples | All |
| What to do about each finding | — | ✓ |
| Architecture plan per library | Summary only | ✓ |
| Export to Excel, history and comparison | — | ✓ |
| Fixes and "make it Copilot ready" | — | ✓ |
| Report | Dapt-branded PDF | PDF and web page, your branding |

[Find out about Pro](https://www.daptgroup.com/solutions/business-apps/site-assessment)

## Install

About 20 minutes. The only admin step is uploading the package.

1. **Upload the app.** In the SharePoint admin centre, go to **More features > Apps > Open**, choose **Upload** and pick `dapt-site-assessment.sppkg`.
2. **Keep it to one site.** Leave **Enable this app and add it to all sites** unticked, then choose **Enable app**.
3. **Add it to a site.** On the site that will host it, go to **Site contents > New > App** and choose **Dapt Site Assessment**.
4. **Add it to a page.** Create a page with a full-width section, add the **Dapt Site Assessment** web part and publish.
5. **Run the scan.** As a **site owner**, open the page and choose **Start the assessment**. Large sites take a few minutes, so keep the page open.
6. **Save the report.** Fill in **Prepared by**, choose **Report (PDF)** and then **Save as PDF**.

You can also type the address of another site on the same tenant to assess it, as long as you have access to that site. The setting **Let people assess other sites** turns this off.

## Security and privacy

- **Read-only.** It never creates, changes or deletes anything in SharePoint, and it makes no lists.
- **Runs as you.** It uses the SharePoint REST and search APIs with your own permissions, so it only sees what you can see.
- **No admin consent.** It needs no Microsoft Graph permissions, no API approvals and no Azure.
- **Results stay in your browser.** They're worked out on the page and disappear when you close it. Dapt receives nothing unless you send us the report.
- **Links to Dapt.** The "Talk to Dapt" links open daptgroup.com and pass only the site's grade and score, and only when you click.
- **Settings panel telemetry.** The settings panel uses the open-source PnP property controls. When someone edits the web part, these may send anonymous usage counts (control name and version, never your content) to the PnP project.
- **The report contains site details.** The saved report includes file names, folder paths and people's names. Store and share it like any internal document.

## If something looks wrong

| What you see | What to do |
| --- | --- |
| "You aren't an owner of this site" | Run it as a site owner or site collection admin to get the full picture |
| "Never opened" shows a dash | Search hasn't indexed the site yet. Carry on; it's a hint, not a measure |
| The scan slows down | SharePoint is throttling. Leave it running; it waits and carries on |
| It stops at 300,000 items | That's the limit for one scan. Assess big sites a section at a time, or ask about Pro |

## Removing it

Remove the page, then remove the app from **Site contents** and the App Catalog. Nothing else is left behind.

## Version history

| Version | Date | Changes |
| --- | --- | --- |
| 1.2.0 | 9 Nov 2026 | First public release of the free edition: no licence key, nothing sent outside your tenant by the scan, 5 examples per finding, PDF report |
