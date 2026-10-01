# Privacy Policy

*Applies to: "doDev – Admin & Dev Toolkit for Salesforce" (the "Extension").*
*Last updated: 1 October 2026*

## Summary
The Extension runs entirely inside your browser. It reads information from the Salesforce org you are already logged into, shows it to you, and then forgets it. **We do not collect, store, sell or send your data anywhere.**

## What the Extension accesses
- **Your Salesforce session cookie** (`sid`), only on Salesforce domains. It is used to call the Salesforce APIs of *the same org it belongs to*, exactly as your browser already does when you use Salesforce. The session is never sent to any other website or server.
- **Salesforce data you ask to see**: for example, profiles, permission sets, users, sharing, metadata, source code, licences and queues. The Extension requests only what is needed for the comparison or report you run.

## What the Extension does NOT do
- It does not send any data to the developer or to any third party. There are no analytics, trackers, advertising or remote servers.
- It does not store Salesforce data or your session. Results exist only in the open page and are gone when you close it. The Extension sets no cookies of its own. It adds nothing to Salesforce pages; it opens only when you click its toolbar icon.
- The only things kept are for the Data Explorer, in your browser's local storage on your computer: **saved queries** (the query text and a name you give it) and a **query history** (the text of your last 100 queries, the object name, org name, time and row count). The workspace also keeps, in the same local storage: your **recent runs** of each tool (only the inputs you chose – names of profiles, users, orgs, the object or record Id – never results), the **last session** (which tools were open, their names and last inputs or query) so it can be restored, the Compare Code & Metadata **scope per pair of orgs**, and which places **Where Is It Used** should look in and which **job types** Jobs should show (ticked or not), which **columns** you chose to hide in a results table, and your last 8 **recent searches** from the search box for each org (the name and Id of what you opened – e.g. an object, user or flow – never its data; "Clear" forgets them). **⬆ Import** reads a query file you choose on your computer, only inside the page; **⬇ Export** creates one on your computer. None of this contains Salesforce records; it is never sent anywhere, and it can be deleted in the tool at any time ("Delete", "Clear history") or by clearing your browser's site data.
- It does not change anything in Salesforce, with one exception: **Data Import** creates or updates the records in a CSV file you choose, only after you tick "I understand" and confirm the count and org. It never deletes. Everything else is read-only. Where Is It Used downloads Experience Cloud site definitions with the Metadata API's read-only *retrieve* call; the download is read in the open page and is not saved.
- It does not load remote code.

## Files you create
When you click **Download CSV**, **Gap permission set**, **Copy** or **Print**, the file or text is created locally on your computer by your browser. What you do with it afterwards is up to you.

## Permissions and why they are needed
| Permission | Why |
|---|---|
| `cookies` | Read your existing Salesforce session cookie so the Extension can call the Salesforce API as you, without asking you to log in again. |
| Host access to Salesforce domains (`*.salesforce.com`, `*.force.com`, `*.cloudforce.com`, `*.salesforce-setup.com`, `*.visualforce.com`, plus Salesforce Government Cloud `*.salesforce.mil`, `*.force.mil`, `*.cloudforce.mil` and Salesforce on Alibaba Cloud `*.sfcrmproducts.cn`) | Call the Salesforce REST, Tooling and Metadata APIs of your org, and find sessions for other orgs you are logged into (for org-to-org comparison). No other sites are accessed. |

## Limited Use
The use of information received from Salesforce APIs adheres to the Chrome Web Store User Data Policy, including the Limited Use requirements. Data is used only to provide the features you use, is never transferred to others, and is never used for advertising or to determine credit-worthiness.

## Children
The Extension is a professional tool and is not directed at children.

## Changes
If this policy changes, the updated version will be published at the same address with a new date.

## Contact
Questions about this policy: open an issue at https://github.com/Boopathirajappan/doinit-orglens-community/issues (please do not include any Salesforce data).
