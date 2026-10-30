Salesforce Repository Naming Standard
Repository inventory and proposed names
Purpose
This document lists the Salesforce source repositories in the Wintrust GitHub organization and proposes a consistent naming standard for them. A common standard makes repositories easier to find and search, shows at a glance which Salesforce org each repository belongs to, and gives new repositories a clear pattern to follow.
Naming standard
Each Salesforce repository follows the pattern salesforce-<key>. The prefix salesforce- is fixed and groups all Salesforce repositories together in GitHub search and in alphabetical lists. The key is a short, lowercase identifier for the Salesforce org the repository deploys to. Keys use lowercase letters, numbers, and hyphens only, stay under 40 characters, and do not change once assigned. A purpose suffix, such as -integrations, may be added only when one org needs a second repository.
Repository inventory
The table below lists each current repository, the key assigned to it, and the proposed new name.
No.
Current Repository Name
Organization Key
Proposed Repository Name
1
Deep-Blue-Salesforce-CRM
deep-blue
salesforce-deep-blue (to be confirmed)
2
Commercial-Finance-Salesforce
commercial-finance
salesforce-commercial-finance
3
Fif-US-Salesforce
fif-usa
salesforce-fif-usa
4
VeteransFirst
veterans-first
salesforce-veterans-first
5
Specialty-Finance-Salesforce
specialty-finance
salesforce-specialty-finance
6
WintrustLifeFinance-Salesforce-CRM
wintrust-life-finance
salesforce-wintrust-life-finance
7
GLA-Salesforce
gla
salesforce-gla
8
Fif-CANADA-Salesforce
fif-canada
salesforce-fif-canada
9
CDEC-Salesforce
cdec
salesforce-cdec

Notes on the proposal
The key for each repository is based on the business unit or entity named in the repository description. Where the description does not name an org, the key is marked for confirmation. Deep-Blue-Salesforce-CRM is the main example: its description does not identify the business unit it serves, so the proposed name must be confirmed with that team before any change is made.
Before any rename, each key should be checked against the Salesforce org alias used in the SFDX project, so that the repository name, the org alias, and the deployment targets in CI/CD stay aligned.
Next steps
Confirm the key for each repository with its owning team. Confirm the Deep-Blue key. Rename one repository first and verify that pipelines, local clones, and branch protection rules still work. Once the pilot is complete, rename the remaining repositories in one change window and publish the standard for future repositories.
