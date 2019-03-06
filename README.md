# GTM Documentation
Example container, naming conventions and setup guidelines for Purdue University, Polytechnic Institute

## Example Container
The file "initial_pu-ppi_tracking.json" is an example container that includes the following initial tags and triggers:

PU GA page views 
PPI GA page views and events to match previous GA embed codes.
* downloads
* mailto link clicks
* webform submissions
* outbound link clicks

To use the file, import it into your workspace and change the "ppi ga account" variable to match your GA tracking ID number. It is customized to match the default Drupal Google Analytics module settings to track events. It also includes auto tracking of submitted forms as events. This is based on the "Webform" module structure with unique form IDs.

## Naming Conventions

### Capital vs lowercase names
Use lower case to identify custom tags and variables you create. Reserve Case for pre-defined tags and variables. This allows us to quickly determine who made what, and will help identify where problems may have originated from.

### Tags, Triggers and Variables
Include the site the tag is for, the GA account data is being sent to, and the track type or actual event.

#### Example tags for sending pageviews to two GA accounts and an event that sends outbound link clicks to the ppi GA account:
* ppi ga - ppi pageview
* pu ga - ppi pageview
* ga event - ppi ga - outbound link click

### Folders 
Use folders to collect items for separate GA accounts and global variables and triggers. Example:
* global
* ppi 
* pu

### Variables
Use constant variables when available. This will reduce redundancy and help keep multiple GA accounts separate.

Example variables for defining two GA accounts:
* ppi ga account
* pu ga account

### Data Layers
Be consistent with use of data layer variable names. Proposed naming conventions:

#### Event Category:
* Webform Submission - Event Action: "Unique Form ID/Name" - Event Label: "Submission URL"
* Outbound links - Event Action: "Click" - Event Label: "destination URL"
* Mails - Event Action: "Click" - Event Label: "destination URL"
* Forms - Event Action: "Click" - Event Label: "destination URL"
* Downloads - Event Action: "Click" - Event Label: "destination URL"

### Reference documentation:
* https://www.analyticsmania.com/post/google-tag-manager-best-practices/
