## HolidayHelpers Client Manager

_This repository strives to be a unified resource in support of the aforementioned web app._

### Table of Contents

1) Why the turmoil? I thought this thing worked 9 years ago...
2) Recent Changes & Outlook for 2022
3) How to Report an Issue
4) Known bugs and interim work-grounds
5) Contacting Owen
6) Changelog Archive


### Why the turmoil? I thought this thing worked 9 years ago...

When the client manager was originally written, PHP 5.6 was the current version.
Now 8.1 is the latest release and 5.6 stopped receiving support back in 2017.

Also, in the 13 years gone by, Javascript has evolved into one of the most popular languages and able to provide user experiences that a server-side language like PHP simply cannot.

As issues arise from the deprecation, those parts are being rewritten using modern code.

We are not switching to PHP8.1 yet, only because that would completely obsolete every third party library we employ. After the site is fully functional again including all requested changes still pending, we will make the switch, with the end result of moving away from PHP wherever we can.

This will inevitably consume the entire season, but I will do my best to keep up with mounting issues as they are reported.



### Recent Changes & Outlook for 2022

#### 11/14/22
 - Layout
   - To speed up fixes and upgrades, the view has been limited to a mobile simulation on Desktop. The ultimate goal is to provide every feature no matter the device.
   - The Vex module popups we were using are being converted to inline elements for user input to cooperate with mobile devices.
 - Fixes
   - Balance sheet loads and shows correct number, and is able to accept payments.
   - Call List (now called Leads) functions again.
   - Several issues with the calendar fixed:
     - Days between start and end are now also shown in the middle days
     - Database connectivity errors
     - Converted several deprecated functions into useable code.
   - Front page active list was not showing up
   - Archive now loads asynchronously with still some work to do for improving workflow and eliminating glitches.
 - Created Support Hub (this) and link via the sidemenu

#### 10/26/22

- Confirming _leads_, formerly the _call list_, and scheduling should now work instead of giving 500 server error.
  - [x] Issue #1: **HIGH PRIORITY**
    - Entering an event spanning 3 _or more_ days will result in only displaying the first and last day on the calendar views
- The menu on mobile phones was not displaying in most situations, should resolved.
- _Vex modals_ are dead and we are no longer utilizing their project. They will be replaced with a non-modal solution keeping inline with a _mobile-first_ approach to user experience design.

  >You will probably find some weird un-vexed popups still. Please report these to me when you do.

### How to Report an Issue

We currently lack a more formal issue tracking software for this project, so just contact me directly as listened below.

Please do not hesitate to contact me at any time with an issue.

- Email
  - _omcalack@gmail.com_
- SMS
  - _**415-484-9379**_
- Mobile
  - **_434-257-6835_** (preferred)

### Known bugs and work-arounds for interim

- [ ] Multiple Issues with Invoices (top priority)
- [ ] Balances (top priority)
- [ ] Display Issues
- [ ] Map Issues
- [ ] Time Clock Issues
- [ ] Mobile vs Desktop Issues

### Contacting Owen

Please do not hesitate to contact me at any time with an issue.

_Find the contact details in the app.._

### Change History

Here is a log of the changes made to the website for the sake of man and woman-kind that are to come.

#### 01-02-2022

- New fully responsive design, optimized with mobile usage in mind
- Menus rearranged, all of the same features exist
- Invoices for jobs have been broken into two separate concepts that will be recorded year to year
  - Estimates - the amount quoted to the customer
    - automatically pretty formatted as pdf able to be emailed, printed, and saved
  - Bills - the final invoice to be paid for by the customer
    - as before, also automatic and pretty
    - will include links/QR Codes to streamline  payment
- New Google Analytics code embedded and working (GA4)
- Innumerable bug fixes.

#### 10-14-2021

- Switched from mysql database code to mysqli
- Begun preparing for our upgrade to php 8 systemwide.
- Continued code re-write to be more modular and upgradeable in the future.
- Switch Google Map to the new Google API (which charges, but has credit, for now)
- Integrated NPM for the basis of our development stack. Also WebPack for the production release.
- Ton of Bug Fixes

#### 9-7-2021

- Implement font-faces into css file that we're using on the website
- Download photoshop plugin to edit favicons, so i can fix favicon being the incorrect aspect ratio

####  9-3-2017

- Change log created to document and track effective progress over time.
- Installed Compass and SASS for project. Two bits of software that aid in the development of creating easy to read
and manage responsive stylesheets.!
- Installed new Google Analytics project tracking code on the new version of the site, and configured
Google Analytics to track and report the most relevant data we will most likely use in the future. (This can always be
adjusted in the future as our needs for data collection and parsing may change.)
- Found and downloaded required fonts requested to be included in the website design by Caleb. Implemented the necessary
code that is required to interject custom web fonts into the website's design, and configured the fonts as was
necessary.
- Started parsing through CSS code from Liquidators' site and copying over tags, classes, and other shit to reuse
