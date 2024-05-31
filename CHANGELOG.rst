=========
Changelog
=========

unreleased
==========


1.6.1 (2024-05-31)
==================
* fix: add `data-popup="yes"` to the link with class `related-widget-wrapper-link`, then the popup will be shown when the user clicks on the link. 
  The JS logic got changed after Django 4.1 upgrade (#15301)


1.6.0 (2024-05-16)
==================
* addd support for django 4.2
* add support for Python 3.10
* drop support for django < 3.2


1.5.0 (2022-09-13)
==================
* feat: Changed compliance number length to 30 characters

1.4.3 (2022-07-08)
==================
* fix: broken pop ups not closing on save

1.4.2 (2022-07-07)
==================
* fix: Fixed inconsistency in Content Expiry form field UI behaviour for the compliance number

1.4.1 (2022-07-06)
==================
* fix: Fieldsets should remain in the same order when compliance number is read only

1.4.0 (2022-06-29)
==================
* feat: Expiry field removed from version table and replaced with compliance number. Added additional content settings action to version table
* fix: Changed model title to uppercase
* fix: Compliance number should not be editable when version is not draft

1.3.1 (2022-06-22)
==================
* feat: Adding functionality to copy a compliance number to all items in a collection

1.2.1 (2022-06-20)
==================
* fix: Compliance number filter input limited to 15 characters

1.2.0 (2022-06-17)
==================
* feat: Compliance number filter added
* feat: Compliance number added to list display and csv export

1.1.0 (2022-06-15)
==================
* feat: Change view title and icon tooltips name changed
* feat: Added compliance number field

1.0.0 (2022-04-25)
==================
* Python 3.9 support added
* Django 3.0, 3.1 and 3.2 support added
* Django 1.11 support removed

0.0.8 (2021-11-26)
==================
* fix: Polymorphic models incorrectly showing in the Default Content Type model configuration form

0.0.7 (2021-11-24)
==================
# feat: Data migration now has a fixed date option that allows the user running the command to provide a datetime and provide a custom format
* fix: CSV Export contains the polymorphic content type when it shouldn't

0.0.6 (2021-11-23)
==================
* fix: Content Expiry Changelist: Removed polymorphic model support due to persistant timeouts and low performance

0.0.5 (2021-11-16)
==================
* fix: Content Expiry Changelist: Timeouts due to Content Type filtering by polymorphic models using the full data set.

0.0.4 (2021-11-08)
==================
* feat: Content Expiry Changelist Content Type filter: Handle filtering by polymorphic models such as filer image / file.

0.0.3 (2021-11-05)
==================
* feat: Filter the Content Expiry Changelist PageContents and Alias Content Type by site, the feature can also be used by other third party packages to restrict the entries shown in the changelist.

0.0.2 (2021-11-01)
==================
* fix: Provide content links in the Content Expiry changelist and csv file export
* fix: Content Expiry changelist filter dates should be for the future not the past
* fix: CSV export Dates are not formatting correctly in Excel
* fix: CSV export external urls used for for the url column

0.0.1 (2021-10-04)
==================
* Initial release
