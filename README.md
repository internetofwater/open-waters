# Open Waters

## What is Open Waters?
Open Waters is a web-based water quality data management system that allows you to manage water quality monitoring locations, samples, results, and projects. The intended audience is tribal, state, or local volunteer water quality data managers, who collect and manage water quality data, and have the need to submit this data to EPA's WQX program. Open Waters is unique in that people can manage their data locally, but submission to EPA is completely automated and handled behind-the-scenes, thus eliminating the burden of separate data submission to EPA. Plus, it is free and completely open source.

## File Downloads
* Full Installation Package - Version 1.7.2 http://www.open-environment.org/downloads/OpenWatersFullInstall_v1.7.2.zip
* Patch Installation Package - Version 1.7.2 - only use this if you are upgrading from version v1.6 to v1.7x http://www.open-environment.org/downloads/OpenWatersPatchOnly_v1.7.2.zip
* User's Guide - Version 1.7 http://www.open-environment.org/downloads/UsersGuide.docx

## Open Waters Features

* Water Quality Data Management: Manage your water quality samples & results, monitoring locations, projects, and organizations, including biological metrics and indices.
* Automatic WQX Submission: Data is automatically submitted to EPA’s WQX program (http://www.epa.gov/storet/wqx/) as it is entered (if data is flagged for submission to EPA)
* Reference Data Synchronization: Reference data (e.g. Pollutant names, Taxonomic names, analytical methods, etc) are fully synchronized with EPA’s reference data, ensuring that submissions will not fail due to mismatches in reference values.
* Bulk Data Import: Data can be bulk imported from Excel, saving time on data entry.
* Charting: Time series charts can be generated with a variety of options.
* Mapping: View monitoring locations geospatially and see latest sampling results. Publish public map.
* Application Customization: Customize app to show or hide various data elements, allowing application administrator to streamline data entry to only include the data elements of interest to the Agency staff.
* Security: Role-based application security and additional layered security measures to ensure data security
* Multi-Organization Support: Support multiple agencies to share the application; all data is segmented by Organization.
* Open Source: Application is free to use, free to share, and free to modify License: GNU GPL v3


## More Information and Example Screens
* More information can be found at: http://open-environment.org/open-waters

## Prerequisites
Web Server
Windows Server 2003 or later (IIS 6 or later)
.NET Framework 4.5
Microsoft WSE 2.0 & 3.0
web server can communicate with Internet and Database (no firewall prohibiting access to EPA’s WQX server)
Database Server
SQL Server 2008 or later (Express edition is OK)


## Change Log
<ul><li><strong>12/23/2015</strong> Version 1.8 released: </li><ul>
<li>Added import translations: now before importing data you can define a mapping of your data to EPA acceptable data. This is helpful in cases where you receive 
data from labs using codes different from EPA and don't want to have to update the import spreadsheet every time. </li>
<li>Additional code cleanup </li>
</ul>
</ul>
<blockquote>----1.8.1 update 
</blockquote><ul><li>Add validation for entering monitoring locations.</li>
<li>Add ability to set default Sample Fraction when importing using cross-tab templates </li>
<li>Add ability when importing cross-tab to handle empty columns</li>
</ul>


<ul><li><strong>6/5/2015</strong> Version 1.7 released: </li><ul><li>MINOR ENHANCEMENTS:  </li><ul><li>Sample result import validation enhancement: sample fraction required for certain characteristics </li><li>Better error message when creating new user and email server not configured properly </li><li>Admin --&gt; Data Synch --&gt; updated to new URL for pulling Org list from EPA </li><li>Bug fix: Fix collation error in create database script for REF_DATA table. </li><li>Fix display issues when using Internet Explorer Version 7 or Compatibility View </li><li>Fix monitoring location edit page to pull counties drop-down from county reference table  </li><li>Better error handling when importing crosstab and monitoring location is missing </li><li>Updated Installation/Users Guide  </li></ul>
<blockquote>----1.7.1 update 
</blockquote><ul><li>Fix bug on Activity Edit page </li><li>Add warning for users if they attempt to enter data before making the initial pull of reference data from EPA </li></ul><blockquote>----1.7.2 update 
</blockquote><ul><li>New data filter added to Activity Search Page: WQX Submit status </li><li>When submitting to EPA and a record fails, error report now displays in human-readable format instead of XML report  </li><li>Additional data validation on import samples </li><li>Bug fix: WQX submission history page not displaying when accessed via Activity page </li><li>Bug fix: handle situation where ResultStatus<a href="/p/open-waters/w/edit/ResultStatus">?</a> or ValueType<a href="/p/open-waters/w/edit/ValueType">?</a> is empty string when submitting to EPA </li></ul></ul><li><strong>5/4/2015</strong> Version 1.6.2 released:  </li><ul><li>Improvements to Crosstab Import Template Configuration Page: characteristic, unit, and activity ID drop-downs added </li><li>Added new help page </li><li>Updated Installation/Users Guide </li><li>Fix import from cross tab when no Activity Type or Activity Media provided to show correct error message. </li><li>Cross-tab Activity Data Import Enhancement: new option to include seconds when autogenerating activity ID  </li><li>Activity Data Import Enhancements: when detecting column data based on header text: (A) now case-insensitive (B) system can now detect column header alias names for certain columns </li><li>Activity Data Import Enhancements: when importing data that already has matching activity ID's added option to either replace or append to existing data </li><li>WQX History page expanded: now can also display records pending for WQX transfer and now available for non-global admins </li><li>Charting Page Improvements: added ability to filter only data shared with EPA; fix monitoring location drop-down;  </li><li>Public map improvement: added organization to popup window; add organization data filter </li><li>Activity Details Page: added ability to view/edit more result fields (Laboratory, Lab Sample Prep Method, Prep Date, Dilution Factor) </li></ul></ul>
<ul><li><strong>4/3/2015</strong> Version 1.6 released, a major update which includes: </li><ul><li>MAJOR ENHANCEMENTS:  </li><ul><li>New 'Getting Started Wizard' guides users through the initial startup steps (creating an organization, getting your organization provisioned, configuring default data values, importing data). </li><li>ew Data Import from EPA-WQX feature: You can now import monitoring locations, projects, and activities directly from EPA-WQX. This is helpful when getting started with Open Waters in situations where you already have data at EPA-WQX. </li><li>Greatly expanded Activity Import from Excel: now supports the import of most 100+ activity/result fields for chemical and biological monitoring </li><li>Greatly expanded Activity/Result Edit page: 20+ new fields added (sample collection method, analytic method, sample collection equipment, activity depth, biological monitoring fields, result status, sample fractions, lab analysis date, time zone, etc.) </li><li>Deleted data synchronization: deleted records are now synchronized with EPA-WQX </li><li>Self-Registration option: Added option (which can be turned off) that allows users to self-register their Open Waters accounts </li><li>Improved Organization-level Security: Users can now make a request to join an organization. Organization or global admins are notified on the dashboard when a request is made, where they can approve/deny access. </li><li>Activity Search page improvements: display Monitoring Location, Project, and Samp Collection Method; add paging; remember search criteria; drop-downs now limited to your selected Org </li><li>Reference Data Enhancements: </li><ul><li>10 additional reference lists now synched with EPA (Method Speciation, Thermal Preservative Used, Cell Form, Cell Shape, Bio Assemblage, Bio Intent, Habit, Voltinism, and Statistical Base Code, Frequency Class Descriptor) </li><li>4 organization-specific reference lists added (Laboratory, Analysis Method, Sample Collection Method, and Sample Prep Method) </li><li>Reference data search feature added </li></ul><li>New Organization Default Data screen added: allows orgs to define the characteristics, taxa, units, detect limits, analytical methods, and time zone used by their organization, which speeds up subsequent data entry. </li></ul><li>MINOR ENHANCEMENTS:  </li><ul><li>Cloud-based emailing: server admins now have the option to send emails using www.sendgrid.com (3rd party cloud-based emailing provider) if you don't have your own SMTP  </li><li>Beta invite option: added option to allow system administrator to require beta invites codes in order to register an account.  </li><li>Improved timezone handling: new Organization default value and automatic determination of daylight savings based on actvitiy date </li><li>Improve performance of WQX data submittals (only download from EPA when submit fails) </li><li>Mon Loc Import from Spreadsheet Enhancement: now supports option to import county/state/country by either code or name </li><li>Cleaned up storage of application settings. </li><li>Fixed error in handling of county codes  </li><li>Added ability for global admin to import reference data for a single table instead of all tables  </li><li>Update .NET Framework from 4 to 4.5 </li><li>Fix units in dropdown not in alphabetical order </li></ul></ul></ul>
<ul><li><strong>12/14/2014</strong> Version 1.5 released, a major update which includes:  </li><ul><li>New feature: batch import for monitoring locations and samples </li><li>Configure batch import templates </li><li>Example Excel templates for monitoring location, sample, and bio metrics added </li><li>Added analytical methods to EPA data import </li><li>Many bug fixes and usability improvements </li><li>Improved security </li></ul><li><strong>11/27/2014</strong> Version 1.4 released, which includes:  </li><ul><li>Supports organization-specific Exchange Network submission credentials </li><li>XML submission performance improvements   </li></ul><li><strong>1/9/2014</strong> Version 1.3 released, which includes:  </li><ul><li>Better support for using multiple organizations: </li><ul><li>Organization-specific application security </li><li>Organization-specific reference data   </li></ul><li>Added ability to define a subset of commonly-used characteristics (to speed up activity data entry) </li><li>Added option to delete or inactivate monitoring locations   </li><li>Updated documentation </li><li>Minor tweaks </li></ul><li><strong>8/20/2013</strong> Version 1.2 released which adds the following:  </li><ul><li>New Mapping Page: view a map that displays your monitoring locations and most recent monitoring results. Includes both a private map (only available to your staff) and public map  </li><li>Updated Styling: updated user interface </li></ul><li><strong>4/2/2013</strong> Version 1.1 released which fixes several bugs  </li></ul>

