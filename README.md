# SitStartCharts Football

A single-page fantasy-football start/sit prototype. The player pool and projections are sample data; this page does not connect to live NFL data or ESPN.

## Changes

| Area | Before | Now | Why |
| --- | --- | --- | --- |
| Visual design | Dark, green-accented dashboard built from the starter layout | Light matchday scouting sheet, dark scoreboard header, condensed display type, and separate start/lean/sit colors | Make the redesign visibly distinct and improve scanability |
| Data status | The page was labeled “Student exercise” and the sample-data limitation was easy to miss | A visible notice says projections are demos and there is no live ESPN connection | Set accurate expectations before users rely on the numbers |
| Watchlist | Josh Allen and Lamar Jackson were preselected; changes lasted only for the current page session | Starts empty; starred players persist in this browser and can be removed or cleared | Let users build their own list without pretending it matches an ESPN roster |
| Roster setup | Players had to be starred one at a time | “Import names” accepts pasted names, adds matches from the sample pool, and reports names it cannot find | Make manual roster setup faster without implying ESPN integration or hiding missing players |
| Player details | Position metrics had little visual separation | Metrics display as a two-column set of labeled tiles | Make the expanded breakdown easier to read |

## Testing Notes

- In the local page, position filters and player search are easy to find; starring a player adds them to the watchlist, and the selection survives a page reload.
- The roster import was tested with two names in the sample pool and one missing name: it added the two matches and identified the missing name. The original browser watchlist was restored after testing.
- The sample projections can be mistaken for real recommendations. The new demo-data notice makes this clearer, but the numbers remain fictional.
- On `sitstartcharts.com`, the Football control opens `/football`; the position filters and player star are easy to find. Adding a player updates the My Team count, and the page says the list is saved in this browser; sign-in is offered to keep it across devices.
- The live site's Baseball page calls this feature “My Watchlist,” while Football calls it “My Team.” The distinction may be confusing. There is no ESPN roster import, and starring a player does not prove that they belong to the user's ESPN team.
- I could not build a list matching the user's ESPN team because no roster was provided and the site was not signed in. The local “Import names” feature is separate from `sitstartcharts.com` and does not change the live site.