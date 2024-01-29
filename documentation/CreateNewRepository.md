### Repository

* Create new repository:
  * Open Template_Lead_Repository in GitHub
  * Select button "Use this template" with "Create a new repository"
  * Select owner "camaraproject"
  * Insert repository name and a description (following the pattern of the exisiting Sub Projects)
  * Select option "Public
  * Select button "Create repository"
* Add branch rules:
  * Select "Settings" --> "Branches"
  * Select button "Add branch protection rule"
  * Insert "main" as pattern name
  * Select option "Require a pull request before merging"
  * Select option "Require approvals"
  * Select option "Dismiss stale pull request reviews"
  * Select option "Require review from Code Owners"
  * Select button "Create"
  * Select button "Add rule" and repeat it with pattern "*release*"
* Add individuals:
  * Select "Settings" --> "Collaborators and teams"
  * Add maintainers with reading permission
  * Add code owners with writing permission
* Change CODEOWNERS file:
  * Add a line `* @<code owner> @<code owner> ...` at the end of the file
* Change MAINTAINERS.MD file:
	* Insert all maintainers
* Update README.MD
	* Replace all occurances of §...§ adequately
	* Define the value for §api_family_abbreviation§

### Mailing List

* Create Mailing Subgroup:
	* Choose "Create Subgroup" in https://lists.camaraproject.org/g/main/createsubgroup
	* Insert value for "sp-§api_family_abbreviation§" and a description (following the pattern of the existing Subgroups)
	* Select button "Create Subgroup"
	* Select "Admin" --> "Settings"
	* Select "Group Type and Moderation"
	* Select option "Restricted Membership"
	* Select button "Update Group"
	* Add all maintainers and code owners to the mailing list

### CAMARA Website

* Add sub website to CAMARA website
	* Select "Pages" and then one of the existing sub websites
	* Switch to classic mode
	* Copy code in first big text box
	* Select again "Pages"
	* Select button "Add New Page"
	* Paste code in first big text box
	* Select button "Backend Editor"
	* Insert title
	* Update content of the sub website from GitHub Readme.md
	* Select button "Publish"
	* Update Menu including the new sub website

### CAMARA presentation

* Update CAMARA presentation
	* Insert new Sub Project in Overview slide
