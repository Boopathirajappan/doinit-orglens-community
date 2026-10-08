# Privacy Policy

*Applies to: "doDev – Admin & Dev Toolkit for Salesforce" (the "Extension"), published by doInit Tools.*
*Last updated: 7 October 2026*

## Summary
The Extension runs entirely inside your browser. It reads information from the Salesforce org you are already logged into, shows it to you, and then forgets it. **We do not collect, store, sell or send your data anywhere.**

## What the Extension accesses
- **Your Salesforce session cookie** (`sid`), only on Salesforce domains. It is used to call the Salesforce APIs of *the same org it belongs to*, exactly as your browser already does when you use Salesforce.
- **Salesforce data you ask to see** – for example profiles, permission sets, users, sharing, metadata, source code and records. Only what the tool you run needs is requested.
- **Your Salesforce user's time zone and the org's theme colour**, so dates and colours look the way Salesforce shows them.

## What the Extension does NOT do
- ✗ No data is sent to us or to any third party – there is no server of ours at all.
- ✗ No analytics, tracking, advertising or remote code.
- ✗ No connected app and nothing installed in your Salesforce org.
- ✗ Your session is never saved, and Salesforce records are never saved.
- ✗ Nothing is added to Salesforce pages – the Extension opens only when you click its toolbar icon.
- ✗ No cookies of its own.
- ✗ Nothing in Salesforce is changed, except when you choose to import or update records (see *Data you put in*).

## How your data is protected
| Protection | What it means for you |
|---|---|
| **Locked to your own orgs** | Every request is checked before it is sent: it must be HTTPS and go to a Salesforce org you are logged into in this browser (the org you opened the Extension from, or another org you are logged into for org-to-org comparison). Requests to any other address are refused. |
| **No redirects followed** | If a reply tries to send the request somewhere else, it is stopped – the session can't be passed on. |
| **Browser-level block** | The Extension's content security policy lets its pages connect to Salesforce domains only, so even a fault in the code could not send data to another site. |
| **Session only where it belongs** | The session is sent only in the request to the org it belongs to – never in a cookie to another site, never in a web address, never written to disk by the Extension. |
| **No remote or injected code** | All code is inside the Extension package; nothing is downloaded or evaluated at run time (`script-src 'self'`, no `eval`). |
| **Safe display of data** | Salesforce data is always shown as plain text, never interpreted as HTML, so a record value can't run code in the page. |
| **Encrypted on your computer** | The few things kept (below) are encrypted with AES-256-GCM. The key is created on your computer and the browser keeps it so it can be used but not read out. |
| **Checked messages** | The Extension's own pages only accept messages from each other. |

## What is kept on your computer
Only these, encrypted, in your browser's storage for this Extension – never Salesforce records, and never sent anywhere:

| What | Details | How to remove it |
|---|---|---|
| Saved queries | The query text and the name you give it | *Delete* in ☆ Saved |
| Query history | Your last 100 queries: text, object, org name, time and row count | *Clear history* |
| Recent runs | The inputs you chose in each tool (e.g. names of profiles, users or orgs, an object or record Id) – never results | The × next to each one |
| Last session | Which tools were open, their names and last inputs or query, so they can be restored | Close the tools |
| Recent searches | Your last 8 searches in the search box per org (the name and Id of what you opened) | *Clear* |
| Preferences | Compare Code & Metadata scope per pair of orgs, which places Where Is It Used looks in, hidden table columns | Change them in the tool |

Clearing your browser's site data for the Extension removes all of this, including the key.

## Data you put in
- **CSV files and pasted rows** (Data Import) are read inside the open page only – they are not uploaded anywhere except, when you confirm, as the records you chose to create, update or delete in your org.
- **Data Import and Perform update** are the only features that change Salesforce. They show a preview and a check first, and nothing is saved until you check "I understand" and confirm the record count and org. Deleted records go to the Salesforce Recycle Bin.
- **⬆ Import** of a query file reads the file you choose inside the page only.
- **Where Is It Used** downloads Experience Cloud site definitions with the Metadata API's read-only *retrieve* call; the download is read in the open page and is not saved.

## Files you create
**Download** (CSV or Excel), **Copy**, **⬇ Export**, **Gap permission set** and **Print** create the file or text locally on your computer, through your browser. What you do with it afterwards is up to you.

## Permissions and why they are needed
| Permission | Why |
|---|---|
| `cookies` | Read your existing Salesforce session cookie so the Extension can call the Salesforce API as you, without asking you to log in again. |
| Host access to Salesforce domains only (`*.salesforce.com`, `*.force.com`, `*.cloudforce.com`, `*.salesforce-setup.com`, `*.visualforce.com`, plus Government Cloud `*.salesforce.mil`, `*.force.mil`, `*.cloudforce.mil` and Salesforce on Alibaba Cloud `*.sfcrmproducts.cn`) | Call the Salesforce REST, Tooling and Metadata APIs of your org, and find the sessions of other orgs you are logged into (for org-to-org comparison). No other sites are accessed. |

## Limited Use
The use of information received from Salesforce APIs adheres to the Chrome Web Store User Data Policy, including the Limited Use requirements. Data is used only to provide the features you use, is never transferred to others, and is never used for advertising or to determine creditworthiness.

## Children
The Extension is a professional tool and is not directed at children.

## Changes
If this policy changes, the updated version will be published at the same address with a new date.

## Contact
Questions about this policy: email **doinittools@gmail.com** or open an issue at https://github.com/doinittools/doinit-dodev-community/issues (please do not include any Salesforce data).
