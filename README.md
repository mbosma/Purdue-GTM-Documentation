# GTM Documentation
Naming conventions and setup guidelines for Purdue University, Polytechnic Institute

## Naming Conventions

### Capital vs lowercase names
Use lower case to identify custom tags and variables you create. Reserve Case for pre-defined tags and variables. This allows us to quickly determine who made what, and will help identify where problems may have originated from.

### Tags, Triggers and Variables
Include the site the tag is for, the GA account data is being sent to, and the track type.

Example tags for sending pageviews to two GA accounts:
* ppi ga - ppi pageview
* pu ga - ppi pageview

### Folders 
Use folders to collect items for separate GA accounts.

### Variables
Use constant variables when available. This will reduce redundancy and help keep multiple GA accounts separate.

Example variables for defining two GA accounts:
* ppi ga account
* pu ga account

### Data Layers
Be consistent with use of data layer variable names. Proposed naming conventions:
Event Category:
* Webform Submission - Event Action: "Unique Form ID/Name" - Event Label: "Submission URL"
* Outbound links - Event Action: "Click" - Event Label: "destination URL"
* Mails - Event Action: "Click" - Event Label: "destination URL"
* Forms - Event Action: "Click" - Event Label: "destination URL"
* Downloads - Event Action: "Click" - Event Label: "destination URL"

Reference documentation:
* https://www.analyticsmania.com/post/google-tag-manager-best-practices/
