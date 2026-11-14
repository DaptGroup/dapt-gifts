# Dapt Copilot Advent

A Copilot tip advent calendar for your intranet. Each door holds a Microsoft 365 Copilot tip and a prompt to try. When someone ticks a door off ("I tried it"), Santa's 3D North Pole fills up:

- presents (doors 1–6);
- the nine reindeer (7–15, Rudolph last);
- the sleigh and its kit (16–21);
- Santa himself (22–24).

After all 24 doors, the sleigh takes off and Santa leaves a gift from Dapt.

**Package:** `dapt-advent.sppkg` · **Current version:** 1.0.2 · [Download from Releases](https://github.com/DaptGroup/dapt-gifts/releases?q=copilot-advent)

## Features

- **24 tips, ready to go.** They're based on Microsoft Learn and Microsoft support content, and the lists are filled in the first time you run setup.
- **Make them yours.** A Copilot champion can rewrite any tip in the **Copilot Advent Tips** list. Setup never overwrites your edits.
- **Copy and open Copilot Chat.** One click copies the day's prompt and opens Microsoft 365 Copilot Chat.
- **Ratings and notes.** People can rate a tip and note what they tried. They see only their own notes; site owners see everyone's.
- **Department leaderboard** (optional).
- **Pilot it early.** Set an earlier first-door date to try it before December.
- **Light on the page.** The 3D scene loads only when the calendar is on the page. Without WebGL, or with "reduce motion" turned on, people get a simpler picture and no flight.

## Install

About 10 minutes.

1. **Upload the app.** In the SharePoint admin centre, go to **More features > Apps > Open**, choose **Upload** and pick `dapt-advent.sppkg`. Choose **Enable app**. You can make it available to all sites, or only to the site you'll use.
2. **Pick a site.** Use a communication site that everyone can read, and keep its **members** to owners and your Copilot champions, because members can edit the tips.
3. **Add it to a page.** Edit a page, add the **Dapt Copilot Advent** web part and publish.
4. **Run setup once.** As a site owner, edit the web part and choose **Set up now**. This creates three lists and fills in the tips.
5. **Optional settings:**
   - **First door opens on:** leave it blank for 1 December.
   - **Department leaderboard:** show or hide it.
   - **Preview every door while editing:** check every door before launch.

## Lists created by setup

| List | Who sees what |
| --- | --- |
| Copilot Advent Tips | Everyone reads. Members and owners can edit. |
| Copilot Advent Progress | One item per person (days done, department). Everyone reads it for the leaderboard; people edit only their own. Hidden from search. |
| Copilot Advent Notes | Ratings and notes. People see their own; site owners see all. Hidden from search. |

## Security and privacy

- **No extra permissions.** It needs no Microsoft Graph scopes and no admin API approval. It works with the access people already have to the site.
- **Data stays in SharePoint.** Progress, ratings and notes are kept in the three lists on your site. Nothing is sent to Dapt.
- **Safe links only.** Tip links only show when they go to learn.microsoft.com, support.microsoft.com, adoption.microsoft.com, www.microsoft.com or your own SharePoint. Anything else is hidden.
- **Progress is self-reported.** It's a fun app with nothing to win. Site owners can correct or delete progress items.
- **Settings panel telemetry.** The settings panel uses the open-source PnP property controls. When someone edits the web part, these may send anonymous usage counts (control name and version, never your content) to the PnP project.

## Removing it

1. Remove the web part from the page.
2. Delete the three lists if you no longer want the data.
3. Remove the app from **Site contents** and from the App Catalog.

## Version history

| Version | Date | Changes |
| --- | --- | --- |
| 1.0.2 | 11 Nov 2026 | Copy the prompt and open Copilot Chat in one click |
| 1.0.1 | 11 Nov 2026 | Smoother sleigh landing |
| 1.0.0 | 10 Nov 2026 | First release |
