
## 3.12.78.23

(Includes Resource Scheduling controls version 1.2.19.221374).

- `Msdyn_SearchResourceAvailability` API fix applying territories constraint.
- Updates to new schedule board: 
    - Schedule assistant update to show error message from server side plugin.
    - Schedule assistant use of custom filters.
    - Date picker localization of "Today."
    - Map view support for certain letters (for example: ŁĄŚĆŻĘŃÓŹ).
    - Schedule board loading when no default language is provider (for example: `UiLanguageId` missing in user settings). 

## 3.12.77.18

(Includes Resource Scheduling controls version 1.2.18.221304).

- New schedule board updates to address issues with auto refresh, resource requirement data not populating, time calculation, time zone application, schedule assistance filters.
- `msdyn_SearchResourceAvailability` API update to support territory constraints.

## 3.12.76.1

(Includes Resource Scheduling controls version 1.2.17.221165).

- New schedule board updates to address issues with requirements on map view, drag and drop errors setting duration, and schedule assistance application of booking rules.

## 3.12.75.2

(Includes Resource Scheduling controls version 1.2.16.220914).

- New schedule board fix for preferred resources filter.
- New schedule board fix where the custom filter doesn't clear the existing value correctly.
- New schedule board fix to view all of the items in the drop down when filtering for territories. 
- New schedule board modified the logic to calculate remaining duration and fulfilled duration. 


## 3.12.74.1

(Includes Resource Scheduling controls version 1.2.15.220774).

- Fixed bug: Resource utilization expand and collapse on the new schedule board.
- Fixed bug: `msdyn_SearchResourceAvailability` returned inaccurate time slot type. 
- Improved daylight saving time to avoid invalid date and time errors. 


## 3.12.73.25

(Includes Resource Scheduling controls version 1.2.14.220634)

- Fixed bug: `msdyn_SearchResourceAvailability` API returns wrong results if the search range is in the next hour.
- Fixed bug: Travel time shouldn't be considered when returning available time slots for facility scheduling.
- Fixed bug: `msdyn_SearchResourceAvailability` API should respect existing bookings only return where resource has idle time, and when user checks **Ignore duration** on UI. API should also return slots with less than required duration. 
- Fixed bug: On the new schedule board, filter for bottom requirement section doesn’t work correctly for boolean fields. 

## 3.12.72.9

(Includes Resource Scheduling controls version 1.2.13.220534)

- Fixed bug: On the new schedule board, search range is always two days instead of taking the time range set when using "Find availability."
- Fixed bug: Proper error message is not shown when an unprivileged user is trying to delete a booking from new schedule board. 
- Fixed bug: Quick book is throwing "Cannot read properties of undefined (reading 'from')" error message when: (1) requirement group without from date, and (2) custom entity without from/to mapping.
- Fixed bug: On the new schedule board, date fields on the booking panel use incorrect date format.
- Fixed bug: Booking on the new schedule board doen't reflect booked hours correctly for project team member.
- Fixed bug: On the new schedule board, proper error message is not shown when user is trying to delete a record that has some related booking alert records.  
- Fixed bug: “Date-time format for /Date is invalid or value is outside of supported range" when using retrieve resource query on the new schedule board.
- Fixed bug: Unable to change booking status on the new schedule board. 
- Fixed bug: KPI panel on the new schedule board is not updated when booking suggestions.
- Fixed bug: Race condition when rendering availability slots in SA mode.

## 3.12.71.20

(Includes Resource Scheduling controls version 1.2.12.220462)

- Fixed bug: travel time shouldn't be considered when returning available time slots for facility scheduling.

## 3.12.71.16

(Includes Resource Scheduling controls version 1.2.12.220462)

- Fixed bug: Custom booking template for custom entity is not being shown correctly. 
- Fixed bug: Facing error when selecting **Book** option from service activity through quick book.
- Fixed bug: Quick book throws "Cannot read properties of undefined" error for two scenarios: 
  - Requirement group without from date.
  - Custom entity without from/to mapping.
- Fixed bug: On new schedule board, values in start time and end time columns are not in sync with time zone displayed in board view settings when booking a requirement group.
- Fixed bug: New schedule board doesn't remove canceled work items from map.
- Fixed bug: On new schedule board, booking method for the newly created bookings should be set as "Schedule Board."
- Fixed bug: Spinner when searching resources is not showing user-friendly label on new schedule board. 
- Fixed bug: On new schedule board, details panel always takes view ID from default `BookingSetupMetadata(BSM)`.
- Fixed bug: On new schedule board, API to create bookings would fail when using logical name instead of schema name.
- Fixed bug: Legacy schedule board sends a request to `GetAvailabilitySummaryFromDemand` with zero resources, causing performance issue.

## 3.12.70.3

(Includes Resource Scheduling controls version 1.2.11.220252)

- Fixed bug: Default radius value always takes kilometer as calculation unit in the backend when checking resource availability through quick book.
- Fixed bug: Using find availability on new schedule board, values in start time and end time columns of search result page are not consistent with time zone displayed in board   view settings when booking a requirement group.
- Fixed bug: On new schedule board, filter on service account does not list all the possible service account names.
- Fixed bug: On new schedule board, mapped custom fields are not being populated when booking created.  
- Fixed bug: `FpsAction 210` filters out active bookings.
- Fixed bug: On new schedule board, booking tooltip shows different booking record.
- Fixed bug: On new schedule board, pending booking stays on the board if booking creation fails.
- Fixed bug: Creating a booking silently fails if associated requirement record does not have remaining duration attribute set.
- Fixed bug: Find availability does not show error message when booking requirement group if error occurs. 

## 3.12.69.1

(Includes Resource Scheduling controls version 1.2.10.213612)

- Fixed bug: On the new schedule board, resource calendar doesn’t consider time-off hours if configured as time off. 
- Fixed bug: Geocode fails with the error message "ResourceID GeoCode_AddressBadRequest was not found" due to missing label in the localization file. 
- Fixed bug: New schedule board does not filter by date if the date format is not US or ISO and region is non-US. 
- Fixed bug: New schedule board does not filter by custom fields on related entity for requirement view. 

## 3.12.68.8

(Includes Resource Scheduling controls version 1.2.9.213482)

- Enabled **Time Group Detail Start** and **Time Group Detail End** column and sorting on list view when returning results with **Find Availability** functionality. 
- Fixed bug: Resource available hours are not showing correctly on new schedule board when configured calendar with working hours and a time off. 
- Fixed bug: where changing status of booking updated the **Start Time** and **Estimated Arrival Time** incorrectly in some scenarios on new schedule board.
- Fixed bug: Cannot create or update a resource preference to a crew type resource.
- Fixed bug: Time zone conversion issue when select time from time picker on **Search Start** and **Search End** fields when using **Find Availability** on new schedule board.
- Fixed bug: Progress indicator div blocking click events on the booking when define an new booking template. 
- Fixed issue: New schedule board does not filter by date if the date format is not US or ISO and region is non-US.


## 3.12.67.1

(Includes Resource Scheduling controls version 1.2.8.213282)

- Fixed bug: where changing status of booking updated the **Start Time** and **Estimated Arrival Time** incorrectly in some scenarios.
- Enabled fulfillment preference support for single requirement when user uses **Find Availability** to schedule requirement.

(Includes Resource Scheduling controls version 1.2.7.213012)

- Fixed bug: Travel time is included in booking duration when book facility requirement.
- Performance improvement on new schedule board when user uses **Find Availability** to book requirement. 


## 3.12.66.3

(Includes Resource Scheduling controls version 1.2.6.212992)

- Allow users to schedule entities without an associated requirement record with scheduling assistant on the new schedule board. 
- Enabled sorting functionality for new schedule board list view when user uses **Find Availability** to book requirement on hourly view. Users can sort rows using each of the       columns.
- Improved the performance when user uses **Find Availability** to book requirement on new schedule board.
- Fixed bug: Travel time is included in booking duration when booking facility type of requirement on new schedule board. 
- Fixed bug: New schedule board sometimes crashes when scheduling a multiday requirement using **Book and Exit** button with **Find Availability** on the new schedule board. 

## 3.12.65.6

(Includes Resource Scheduling controls version 1.2.5.212813)

- Enabled **Group By** capability on new schedule board list view. 
- On new schedule board, started showing dotted line when user drags-and-drops requirement to the board. 
- Fixed: when update contact record with integration job: Update (Pre-operation) for contact plugin throws Error: **System.ServiceModel.QuotaExceededException: 'The size necessary to buffer the XML content exceeded the buffer quota.'** 		
- Added retry mechanism and logged more information for troubleshooting when Geocode API fails with HTTP 403.

## 3.12.64.78
This release is a hotfix on Universal Resource Scheduling version [3.12.64.46](/dynamics365/common-scheduler/bug-fixes#3126478)

- Added retry mechanism and logged more information for troubleshooting when Geocode API fails with HTTP 403

## 3.12.64.46 - 2021 wave 2 early access general availability 

(Includes Resource Scheduling controls version 1.2.2.212724)

The following Universal Resource Scheduling 2021 Wave 2 features in general availability are included in this release.

- Resource work hours extensibility. 
- Improved user experience with new schedule board enhancements.

This release also includes all the fixes included in the [2021 wave 2 early access](/dynamics365/field-service/field-service-version-history-resource-scheduling#3126043---2021-wave-2-early-access), [2021 wave 2 early access update 1](/dynamics365/field-service/field-service-version-history-resource-scheduling#3126121---2021-wave-2-early-access-update-1) and [2021 wave 2 early access update 2](/dynamics365/field-service/field-service-version-history-resource-scheduling#3126249---2021-wave-2-early-access-update-2).

- Fixed a bug on the legacy schedule board where expanding a pool resource threw an exception. 
- This release contains an update to the new schedule board; now, new schedule assistant and find availability functionality can also be used with the multiday requirements that last for multiple days with associated requirement detail records. We also shipped many experience, performance, and stability improvements. For any schedulable entity to be supported on the new schedule assistant experience, the schedulable entity record needs to have an associated requirement. Support for schedulable entity records without an associated resource requirement record will be added in a future update. A few performance improvements will also be made available on the Schedule assistant and schedule board in future updates. 

## 3.12.62.49 - 2021 wave 2 early access update 2

(Includes Resource Scheduling controls version 1.2.2.2126411)

The release is only applied when an environment is opted into the early access of 2021 wave 1 and introduces the [resource scheduling 2021 wave 2](/dynamics365-release-plan/2021wave2/service/dynamics365-field-service/planned-features#resource-scheduling) new and updated features. 

This release is an update to the 2021 wave 2 early access of Universal Resource Scheduling version 3.12.61.21. 

- There was an issue where Power Automate cloud flow was used to trigger on update of the work order field on the requirement to create a booking for the requirement, but it would create two bookings. This issue is now fixed. 
- When a user clicks on the suggested time slot's resources on the quick book panel, the scroll position is reset and the user has to again click on the available resources of the suggested time slot to see the available resources. This issue is now fixed. 
- This release contains an update to the new schedule board; now, new schedule assistant and find availability functionality can also be used with the multiday requirements that last for multiple days with associated requirement detail records. We also shipped many experience, performance, and stability improvements. For any schedulable entity to be supported on the new schedule assistant experience, the schedulable entity record needs to have an associated requirement. Support for schedulable entity records without an associated resource requirement record will be added in a future update. 

## 3.12.52.4

(Includes Resource Scheduling controls version 1.1.7.211681)

- Fixed an issue where a new booking is created from the booking form directly with a **Booking rule** enabled, the `RequirementId` is not passed via the bookings rule. 
- Made performance improvement on the schedule board by only querying for the active booking records, which are displayed on the schedule board. 
- When booking a multiday requirement, some would get stuck in a loop for a long time when using booking method as **Remaining Requirement** with **Double-book if needed** selected. This issue is now fixed. 
- When the user selects a suggested time slot on the quick book panel, the selection was not highlighted. This bug is now fixed. 
- Fixed **Object reference not set to an instance of an object** error during the upgrade of the environments from an older (v6, v7) version of Field service app to latest v8 versions. 

## 3.12.51.1

(Includes Resource Scheduling controls version 1.1.7.211681)

- When using the API `msdyn_SearchResourceAvailabilityForRequirementGroup` throws an error **Nullable object must have a value.**, when eligible crew has more crew resources than the requirements in the requirement group. This null handling error is now fixed. 
- When a resource has a time off starting from 12 AM, for a few hours, the schedule board is showing that the resource is not working for more than the time-off period. This issue happens for the timezones GMT + x hours. This issue is now fixed and schedule board should reflect the right time-off period. 
- When **Quick Book** is used on a requirement group with only start date and no end date, the quick book window loads forever and shows no results. This issue is now fixed. With this fix the behavior of quick book when used on requirement groups is that: 
	- If there are start and end dates, then the availability is shown accordingly.
	- If there are no start and end dates, then the availability is shown for current date to next 60 days.
	- If only start date is populated, then the availability is shown for start date to next 60 days.
	- If only end date is populated, then the availability is shown for current date to end date.

## 3.12.61.21 - 2021 wave 2 early access update 1

(Includes Resource Scheduling controls version 1.2.1.212252)

The release is only applied when an environment is opted into the early access of 2021 wave 1 and introduces the [resource scheduling 2021 wave 2](/dynamics365-release-plan/2021wave2/service/dynamics365-field-service/planned-features#resource-scheduling) new and updated features. 

This release is an update to the 2021 wave 2 early access of Universal Resource Scheduling version 3.12.60.43. 

- This release contains an update to the new schedule board; now, new schedule assistant and find availability functionality can also be used with the requirement groups. We also shipped many experience, performance, and stability improvements. 
- Fixed a bug: when a user enables the new schedule board toggle and refreshes the browser, the user preference wasn't remembered and they were shown the old schedule board. 
- Fixed a bug: some customers were unable to reimport new custom solutions once they opted into the 2021 wave 2 early access and installed the updates. 
- Fixed non-blocking errors when updates were made to a booking record, like **Sequence contains no matching element**, and **Nullable object must have a value**.
- Fixed issue: Users couldn't drag the resource routes on the schedule board map to a nearby unscheduled requirement to create a booking. In the new schedule board, the user was required to select a resource before letting them drag the route. 
- Fixed issue: When using the new schedule assistant on a work order to book a resource, the work order title was not shown in the header of the schedule assistant experience. 

## 3.12.50.27

(Includes Resource Scheduling controls version 1.1.7.211681)

- Fixed a bug where columns (fields) of type customer would not filter based on the text typed, but show all records, when filtered in column filters on the requirement panel of the schedule board.
- When using the preferred resource on the requirement and quick scheduling is used, incorrect resources are shown with the heart icon for preferred resource. This issue is now fixed. 
- Fixed a bug where an error is thrown when booking end time and actual arrival time are same. This no longer throws an error, as it is a valid scenario for resources. 
- When a resource has time off for a few hours in a day, in the schedule board list view, there are two duplicate line entries for the same time off duration. This issue is now fixed, and should show as only one line item in the list view. 
- Pushed an improvement to the upgrade experience: when an organization deleted an out-of-the box shipped booking status record, the upgrade failed. This issue is now fixed. 
- Fixed an issue where users couldn't create a booking alert that they do not have read and write privileges to the booing alert status record type, even when the user has the necessary privileges but the team they are assigned to doesn't have the privileges. This bug is now fixed. 

## 3.12.60.43 - 2021 wave 2 early access

(Includes Resource Scheduling controls version 1.2.0.212086)

The release is only applied when an environment is opted into the early access of 2021 wave 1 and introduces the [resource scheduling 2021 wave 2](/dynamics365-release-plan/2021wave2/service/dynamics365-field-service/planned-features#resource-scheduling) new and updated features. 

This release also includes the following changes that have the potential to change the existing system behavior or interface. 

- Performance improvements are made when applying the work hours templates to the resource(s). 
- Fixed a bug where the column headers and the columns were misaligned in the list view of the schedule board.
- The tooltip of the **Default radius unit** field of the schedule assistant under Resource Scheduling's scheduling parameter is corrected to **Choose the unit to display the distance on the Schedule assistant experience". 
- When we have the **Derive Capacity From Group Members** set to **Yes** in the **Scheduling Tab** of parent pool resource, any updates to a bookable resource group membership will trigger the deletion of all existing inner calendars of the parent resource and recreate them based on the child resource calendar. This recreation of the inner calendars happens even when we try to add a new child to the pool resource. This takes a lot of time, especially when the time period between the from and to dates is long. The longer the time period between from and to dates, the longer it takes to edit the bookable resource group and can cause the offline or timeout error after a certain threshold. Performance improvements are made by making the deletion of the inner calendars asynchronous. 

## 3.12.49.18

(Includes Resource Scheduling controls version 1.1.7.211681)

- Booking work orders to a resource on the schedule board fails with a null reference error if **Auto Update Booking Travel** feature is not set to a value. This bug is now fixed.
- Fixed a bug on the schedule assistant to calculate the right travel distance of the resource. 

## 3.12.48.25

(Includes Resource Scheduling controls version 1.1.7.211681)

- Booking work orders to a resource on the schedule board fails with a null reference error if **Auto Update Booking Travel** feature is not set to a value. This bug is now fixed.
- Fixed a bug on the schedule assistant to calculate the right travel distance of the resource. 
- Fixed a bug where the schedule board does not load. 
- Fixed a bug where the time zone of the resource was not rendered on the details panel, when a resource is selected. 

## 3.12.47.108

This release is a hotfix on Universal Resource Scheduling version [3.12.47.98](/dynamics365/common-scheduler/bug-fixes#3124798)

- Fixed a bug where the schedule board does not load. 

## 3.12.47.98

This release is a hotfix on Universal Resource Scheduling version [3.12.47.98](/dynamics365/common-scheduler/bug-fixes#3124762)

- Booking work orders to a resource on the schedule board fails with a null reference error if **Auto Update Booking Travel** feature is not set to a value. This bug is now fixed.

## 3.12.47.62

(Includes Resource Scheduling controls version 1.1.6.211322)

- Fixed a bug where the schedule board does not load. 
- Fixed an issue where work hours tab is removed from bookable resource form. 
- When the setting **Auto Update Booking Travel** is disabled, some bookings **Modified On** columns are shown updated when a new booking is created during non working hours for a resource. This bug is now fixed.
- When the field **Estimated Arrival Time** is hidden from the **Information** form of the bookable resource booking entity, updating the **Start time** of a booking record throws an error. This bug is now fixed. 
- Fixed an issue: when two separate bookings in the schedule board were modified in quick succession, it could lead to an issue where duplicate calls were made for the same booking. This issue is now fixed. 

## 3.12.46.64

This release is a hotfix on Universal Resource Scheduling version [3.12.46.21](/dynamics365/common-scheduler/bug-fixes#3124621)

- Fixed a bug where the schedule board does not load. 

## 3.12.46.21

(Includes Resource Scheduling controls version 1.1.6.211322)

- **msdyn_searchresourceavailabilityforrequirementgroup** action sometimes failed with invalid organizational unit locations. This bug is now fixed and will filter the resources to the organizational unit passed even when invalid location is used for the organizational unit. 
- **msdyn_SearchResourceAvailability** and **msdyn_SearchResourceAvailabilityforRequirementgroup** actions are now compatible with the web API endpoints. You could use the API parameter **version** = 3, to use this capability.
- Fixed a bug where columns (fields) of type **Customer** would show both account records and contact records when filtered in column filters on the requirement panel of the schedule board. 
- Improvements were made to the load time of the schedule assistant in the vertical view. 

## 3.12.45.7

(Includes Resource Scheduling controls version 1.1.5.211181)

- When booking a resource from the schedule assistant, on the days, weeks, and months views and using the **Double book if needed** option on the booking panel, clicking on book button would keep the spinner loading without completing the operation. This specifically happened when the resource has no working hour in the duration of the requirement detail. This bug is now fixed. 
- Fixed an accessibility bug on the grid used in the requirement groups. The contrast ratio of keyboard focus on column headers in grid with background is 1.2:1 which is less than required contrast ratio 3:1. This bug is now fixed. 
- Fixed an accessibility bug on the grid used in the requirement groups. At 400% zoom, content inside **Search** popup in **Preferred Resource** column is not completely visible. With this fix, entire content that is visible at default view should be clearly visible at 400%. 
- Fixed a bug where a validation is done on the booking, that the **End time cannot be before or same as the estimated arrival time**, when the actual arrival time is already populated. With this fix, the validation would be that the **End time cannot be before or same as the actual arrival time**, as long as the actual arrival time is populated. 

## 3.12.44.127

- When a booking alert is created in the context of the **SYSTEM** user, an error was thrown that the user does not have create privileges. This bug is now fixed. 
- Fixed a bug where a time tooltip is shown on the hourly view of the schedule board and does not close.
- When schedule assistant is used on onsite requirements with fulfillment preferences of intervals, the end time of the suggested time slot on the list view is shown incorrect. This bug is now fixed. 
- msdyn_searchresourceavailability API returned same GUIDs for all the suggested timeslots when fulfillment preferences are used. This bug is now fixed. 
- In days, weeks, and months views of the schedule board, when new bookings are created or existing bookings are edited, a new visual spinner is shown to represent the progress of the operation. 
- When custom fields of the booking record are displayed on the booking template of the new schedule board, only the schema name of the custom field are displayed instead of the display name of the custom field. This bug is now fixed. 
- Creation of a booking via dragging and dropping of the unscheduled work order on the new schedule board is now supported on the Firefox browser. 
- The available resource names are truncated on the quick book panel, this bug is now fixed. 
- When the requirement view used to display the unscheduled requirements on the schedule board has no sorting defined, an error was thrown. This bug is now fixed. 
- When creating multiday booking using **Evenly Distribute** booking method, user cannot overbook resources with single booking if per-time-period duration is greater than resource's availability during that time. This bug is now fixed. 
- Priority, territory and status lookup fields can now be filtered on the requirement panel of the new schedule board. 
- When the requirement map pins are hidden from showing on the map panel of the schedule board, the requirements were still retrieved in the backend. This bug is now fixed to remove the unnecessary call and improve the load time of the schedule board. 
- Due to different timezones used, the resource availability did not respect the business closure of the resource working hours. This bug is now fixed. 
- Fixed a bug where if user updates appointment series by adding required attendees, new bookings were not created, when (legacy) appointment scheduling feature is enabled. 
- When quick book is used on requirement groups with multiple requirements with the field **Select** = **Any** option, then multiple combinations of same set of resources were shown in the suggested resources. This bug is now fixed. 
- When trying to filter the schedule board to specific resources, it does not filter anything out as **Retrieve Resource Query** field on the schedule board tab was pointing to an incorrect value. This bug is now fixed. 

## 3.12.43.68 - 2021 wave 1 general availability

The following Universal Resource Scheduling 2020 Wave 1 features in general availability are included in this release.

- Map view, weekly, and monthly views in the new schedule board. 
- Appointment data included in resource scheduling.
- Embedded optimizer enhancements within schedule board (preview).

This release also includes all the fixes included in the [2021 wave 1 early access](/dynamics365/common-scheduler/bug-fixes#3124015---2021-wave-1-early-access) and [2021 wave 1 early access update 1](/dynamics365/common-scheduler/bug-fixes#312424---2021-wave-1-early-access-update-1).

- When creating multiday booking using **Evenly Distribute** booking method, user cannot overbook resource with single booking if duration is greater than resource's availability during that time. This bug is now fixed. 
- Fixed a bug where quick scheduling is used on a requirement group with work location set to *Facility*, no available resources are returned. 
- Start and end time on schedule assistant list view mismatches with estimated arrival time and end time on the create resource booking panel when using fulfillment preferences (intervals) are used on aa *Onsite* requirement. This bug is now fixed. 
- **Rebook button** on requirement group’s bookings is using the **Default Booking Committed Status** from default **None** booking setup metadata, rather than using the default booking committed status from the schedulable entity’s booking setup metadata record. 
- **Clear Sorting** option is now available on the column filters of the requirement panel of the new schedule board. 
- When using quick book, the back button on the view resources page disappears if a different date is selected. This bug is now fixed. 
- Business closures are not honored for the resource availability due to the different timezone on the resource work hours and the **User Timezone** preference. This bug is now fixed. 
- When a skill uses a special character like **&** in the name, the skill name is displayed as HTML-encoded in the schedule board filter layout. This bug is now fixed. 
- When using the schedule board’s email driving directions is fixed to send emails to the recipients in the **To** field. 
- When a business closure is created for a day in the Canberra time zone (GMT+10) and saved, the start and end times of the business closure were raised by an hour. This bug is now fixed. 
- Fixed a bug on the new schedule board in Hebrew, where the dates are incorrectly aligned from left to right when next day of the time range is selected. 
- Fixed a bug where schedule board displays text in Chinese on the date columns of the hourly view, when system language is set to Japanese. 
- When using the quick book, and the available resources are accessed on an available time slot, the time displayed is different than the actual time slot. This bug is now fixed. 
- When using a field where time zone information is displayed on the details panel of the schedule board, the field was incorrectly displayed as the time zone code, but not the actual time zone. This bug is now fixed. 
- When a requirement group record is opened from the schedule board requirement panel by double-clicking the record, it threw an error of insufficient privileges. This bug is now fixed. 
- Made an improvement to the date selection on the booking panel of the schedule board. If the start date is selected after the end date, then the end date should also be updated to the start date. If end date is selected before the start date, then the start date should be updated to the selected end date. 
- Unable to complete appointments without system admin security role privileges when customer service scheduling is installed. This bug is now fixed. 
- On the schedule board, we made an improvement to show the booking tooltips, when using the schedule board on a slower network (fast 3G speeds). 
- When a resource requirement record is created, a calendar record is created. When a resource requirement is deleted, additional logic is added to check if the calendar is used by any of the Dynamics 365 out-of-the-box record types, and if the calendar is not used, then the calendar record is also deleted. A similar behavior is also put in place for the work hours templates. This deletion of the calendars improves the performance of the schedule assistant.

## 3.12.42.4 - 2021 wave 1 Early access update 1

The release is only applied when an environment is opted into the early access of 2021 wave 1 and introduces the [resource scheduling 2021 wave 1](/dynamics365-release-plan/2021wave1/service/dynamics365-field-service/planned-features#scheduling) new and updated features.

In addition, this release includes the following changes that have the potential to change the existing system behavior or interface.

- Fixed a bug where the tooltip of a button **Return** on the new schedule board's embedded optimizer, is not localized. 
- Fixed a bug on the new schedule board, where certain bookings with travel time were not shown on the board; only the travel time was shown instead. With this fix, the bookings with travel time are shown as expected on the new schedule board. 
- When details view on the old schedule board is used for resources and a resource view is used where resource timezone is included as a field on the view, the timezone was displayed incorrectly as just a number. This bug is now fixed. 
- When requirement priority name is set to null, the schedule board would throw an error while loading. This bug is now fixed to handle null values on the requirement priority record names. 

## 3.12.40.15 - 2021 wave 1 Early access

The release is only applied when an environment is opted into the early access of 2021 wave 1 and introduces the [resource scheduling 2021 wave 1](/dynamics365-release-plan/2021wave1/service/dynamics365-field-service/planned-features#scheduling) new and updated features. 

In addition, this release includes the following changes that have the potential to change the existing system behavior or interface. 

- Fixed a bug on the new schedule board when a requirement is dragged and dropped into the daily view, the **Create Booking** pane shows incorrect start and end dates. 
- When hovered on disabled buttons on the new schedule board, tooltips were not being shown. This bug is now fixed. 
- When the date format is set to English (United Kingdom), the date fields on the "Create resource booking" pane of schedule assistant were not respecting the above date format selected. This bug is now fixed.

## 3.12.36.2

- Fixed a bug where resources with certain work hours calendar types (type = -1) were not returned by the schedule assistant.
- When the date format is set to English (United Kingdom), the date fields on the create resource booking pane of schedule assistant were not respecting the above date format selected. This bug is now fixed.
- When a schedule board tab’s setting requirement map filter view is configured to a resource requirement entity view that has a view definition including link entity filtering does not contain data, the map view on the tab, does not load. This bug is now fixed. 
- Keyboard navigation and selection issues on the "Characteristics – Rating" filter on the filter view of the schedule board are fixed. 
- When creating bookings for crew type resources using the schedule assistant, the travel times were incorrectly calculated from the organization unit of the crew resources. This bug is fixed, and the travel time is calculated from the location of the crew member resources. 
- When appointment scheduling feature is enabled, non-admin users were unable to mark the appointment record as complete. This bug is now fixed. 
- When certain filter panel customizations were used in the old schedule board, and access the bottom filters of the panel, the filter panel jumps to the top. This jump experience issue is now fixed. 
- When multiple child requirements are defined under a requirement group, there were intermittent timeout issues thrown. We fixed this bug by increasing the timeout duration.
- When apply territory filter setting is selected on the schedule board scheduler settings, on slow networks, this setting was not applying the territory filter on the bottom requirement panel. This bug is now fixed to make the territory filtering on the requirement panel work even in slow or latent networks.

## 3.12.35.6

This release is a hotfix on Universal Resource Scheduling version [3.12.35.5](/dynamics365/common-scheduler/bug-fixes#312355)

- We fixed a bug that impacted the performance of the schedule assistant. 

## 3.12.35.5

- When creating Bookings for Facility type Resources using Quick Book, the travel time is incorrectly added to the total duration of the Booking. This behavior is now fixed, and with the fix, the travel time is excluded from the total duration of the booking for Facility type resources. 
- For geographical regions, where Bing maps has no coverage, (ex: China, South Korea, and Japan), the distance and travel time calculations to the booking locations are calculated to the approximated values via **As The Crow Flies** (ATCF) method. 
- Fixed a bug where, the displayed time range on the schedule Board (old) is less than a day, then Resources routes are not displayed on the Map view. 
- Made some performance enhancements to improve schedule assistant response time. 

## 3.12.34.92

This release is a hotfix on Universal Resource Scheduling version [3.12.34.60](/dynamics365/common-scheduler/bug-fixes#3123460)
- We fixed a bug that impacted the performance of the Schedule assistant. 

## 3.12.34.60

This release is a hotfix on Universal Resource Scheduling version [3.12.34.4](/dynamics365/common-scheduler/bug-fixes#312344)
- Fixed a bug where resources with certain workhours calendar types (type = -1) were not returned by the Schedule Assistant.

## 3.12.34.4

- Fixed a bug where schedule assistant and schedule board ignore start and end time inputs when duration is more than 24 hours when scheduling an opportunity record. 
- Fixed a bug where the search button remains disabled when **Time To Promised** is initially greater than search end, even if parameters are adjusted.
- Fixed a bug where a validation error occurred for `bookableresourcebooking.msdyn_milestraveled`. The value -0.999999690624 of type `System.Double` is outside the valid range (0 to 1000000000). 
- Booking tooltip on multiday views now shows in the correct booking length on the current schedule board and the next-generation schedule board.
- Fixed a bug where the booking is created with an incorrect duration when a user tries to create a booking using the quick book option.

## 3.12.33.8

- When quick book is enabled on a schedulable entity and the requirement record is generated post booking record creation, the from date, to date, and duration attributes on booking setup metadata record were not correctly mapped to the from date, to date, and duration fields of the resource requirement generated. This bug is now fixed.
- When Universal Resource Scheduling is used as the scheduling engine for appointments, and a system user, who does not have an associated bookable resource record, creates an appointment throws an error. This bug is now fixed.
- Fixed a bug on the legacy schedule board, where selecting an empty time slot on the board, and on searching for lookup records, all resource requirement records in the system show up instead of those matching the selected requirement panel at the bottom.
- Fixed an issue where non-admin Field Service users cannot update the Booking records due to insufficient privilege on entity ```msdyn_schedulingfeatureflag```. This bug is now fixed.
- When a booking is canceled on the schedule board and then the work order (or requirement) record is again dragged to the same resource after the canceled booking, the travel time is incorrectly calculated as zero from the previous canceled booking. This bug is now fixed and the travel time is correctly calculated from the previous resource location.
- Fixed an issue where, custom `DateTime` fields from requirement record’s associated entities like work order are not respecting schedule board tab time zone in requirements panel. With this fix, all `DateTime` fields on the requirement panel will be shown in the time zone of the schedule board tab.
- When a work hours template with a time off is applied to another resource, the time-off description and title were not getting copied. This bug is now fixed.
- When a multi-day booking is created with out an associated resource requirement record, changing Booking status on the booking, throws an error, this issue is now fixed.
- The schedule assistant calculates the distance and travel time for the Resources to the booking via the default map provider Bing, this is only enabled when the field “connect to maps” is set to yes. There was an issue where regardless of the value selected, schedule assistant always used the default map provider to calculate distance and travel time. This bug is now fixed.
- Fixed an issue where updates to the bookings of a crew type resource are not made, when booking rules are used. This bug is now fixed. Updates to the crew bookings will be made, even when booking rules are used.
- Fixed scroll jumping issue on the filter pane of the legacy schedule board for certain custom filter panel layouts.
- Fixed an issue where there are multiple time-off hours are used on a single day for a resource, the working hours are not correctly calculated, and so incorrect working hours are reflected on the schedule board.
- Incomplete resource available time slots were shown on the legacy schedule assistant grid view when the fulfillment preferences intervals were used on the resource requirement record. This issue is now fixed, and the complete resource available time slots are shown.
- When quick book is enabled and used, the resource available time slots would respect the "Book based on" setting on the default schedule board settings and will show the resource available time slots based on value chose for **Book based on** - **Estimated arrival time** or **Start Time**.

## 3.12.32.1

 - Fixed a bug on the legacy schedule board, when find **Substitution functionality** is used with in the schedule assistant, the UI was frozen. With this bug fix, **Find Substitution*** functionality can be used with in the schedule assistant mode. 
 - Fixed a bug on the List view mode of the daily view of new schedule board, where changing a booking status doesn’t reflect in the view. Now with the fix, the changed status will also reflect in the list view. 
 - Fixed a bug on the new schedule board where, the resource names are truncated when using right-to-left languages like Arabic. 
 - Fixed a label on the schedule assistant panel to show as **Booking suggestions**. 
 - Additional stabilization improvements were made on the new schedule board to prevent crashes on the board the schedule assistant panel, which is a feature in preview. 

## 3.12.31.50 - 2020 wave 2 general availability

The following Universal Resource Scheduling 2020 Wave 2 features in general availability are included in this release.

- Next generation schedule board experience
- Predictive work duration (Preview)
- Enhanced calendar for requirements
- Embedded optimizer within schedule board (Preview)

This release also includes all the fixes included in the [2020 wave 2 early access](/dynamics365/common-scheduler/bug-fixes#version-312295-2020-wave-2-early-access) and [2020 wave 2 early access update 1](/dynamics365/common-scheduler/bug-fixes#version-3123011-2020-wave-2-early-access-update-1).
- Fixed a bug on the map view of the schedule board, where scheduled requirements with remaining duration equals 0 are still being shown as unscheduled requirement pin, leading to double requirements. With this fix, once a requirement is scheduled and Remaining duration equals 0, the pin will not be displayed as a requirement pin. 
- The days on the daily view of the schedule board are shown in right-to-left orientation for the right-to-left languages like Hebrew, Arabic. 
- Fixed a bug where a new requirement record is created, the status of the requirement record created is not respecting the **Default Requirement Active State** value of the associated booking setup metadata record of the requirement. This bug is now fixed, and the default status of the newly created Requirement record will be based on the default requirement active status of the associated booking setup metadata record.
- When creating a booking for requirement groups using the quick scheduling feature, fixed a bug where the resulting errors (if any) were not surfaced to the end user. Now if there are any errors during the creation of the Bookings, error message will be displayed on the quick book interface. 
- When fulfillment preferences (intervals) are used on requirements, the schedule assistant shows the time slots, and the first time slot will be shown after the **Intervals begin** time. 
- Fixed a bug in the msdyn_SearchResourceAvailabilityForRequirementGroup API, where the last available time slot of a time range are not being returned. 
- Added new additional solution health rules to detect if the following records are missing: 
 - Default schedule board setting.
 - Schedule board setting for the resource utilization view of the schedule board. 
 - Unsupported modification of the OOB web resources.
- When a resource on the booking is substituted with another resource on the schedule board and then find availability is used, fixed a bug where an error was thrown. 
- The date field on the schedule assistant list view is now fixed to respect the date formatting preferences of the user. 
- Fixed a bug where a booking is created using **Find Availability** functionality, and the booking method field is displayed as **Schedule Board**. This is fixed to show the booking method as **Schedule Assistant**.
- Fixed a bug where looking for available resources on the requirement groups, and **Least Busy** option on the schedule assistant is used, Resources returned were not in the right order. This is fixed and only the least busy resources are returned on the top. 
- When preferred resource of resource preferences is used on the resource requirement record, the preferred resources are not returned on the top of the recommended resources using quick scheduling. This bug is fixed, and the preferred resources are returned on the top. 
- Fixed a bug on the schedule board maps view, where the date picker is not displayed when number of days displayed on the board is greater than one. This is now fixed, and the map view will display the date picker to show the map data of a specific day. 
- On the new schedule board, fixed an issue, where a resource is marked as **Display on Schedule Board** as **No**, resource is still being shown on the schedule board.

## 3.12.25.5

- On the daily view mode of the schedule assistant, when **Ignore Duration** advanced setting is selected, all eligible resources were not returned regardless of their availability. This bug is now fixed in this update. 
- Fixed a bug where quick book is used on a requirement group, and resources work in a different time zone than the time zone of the calendar of the requirements in the group, only a part of the available time slots were returned. With the fix, all available time slots are returned in this scenario. 
- When searching for resources in the daily view of the schedule board: once the searched Resources are returned, bookings of the resources are not returned on the center area, until the board is refreshed. This bug is now fixed in this update.
- When a default search radius unit of kilometers is used and no available resources are returned, the schedule assistant crashes. This bug is now fixed, and users can expand the filter panel, even when no resources were returned to change the filters on the filter pane. 
- When quick book is used on a work order with an associated requirement group, and a resource is booked, **Booking Status selected is invalid for Work Order** error is thrown. This issue is now fixed. 
- When looking for available resources on a service activity record and **Least Busy** sort is selected, no available resources were returned. This is now fixed on the schedule assistant. 
- Quick book will honor the default resource search radius defined on the booking setup metadata record of the schedulable entity (for example, work order, case, resource requirement, and so on).
- When any changes are made to a booking (like moving the booking or reassigning the booking), the custom booking rules defined by the user would get triggered. But extending  existing booking would not trigger the booking rule. This bug is now fixed. 
- When fulfillment preferences (intervals) are used with a requirement group, the start date of the schedule assistant filter pane is populated incorrectly, which is now fixed in the update. 
- Schedule board center-area grid is misaligned when browser zoom is changed to 80 percent or 110 percent on Microsoft Edge and Google Chrome browsers. With this fix, the misalignment of the grid is fixed. 
- Fixed a bug where a custom entity cannot be enabled for scheduling, when the name of the entity has more than 100 characters. With this fix, any entity that has a name with more than 100 characters can also be enabled for scheduling. 

## 3.12.30.11 - 2020 wave 2 early access update 1

The release is only applied when an environment is opted into early access and introduces the [resource scheduling 2020 wave 2](/dynamics365-release-plan/2020wave2/service/dynamics365-field-service/planned-features#scheduling) new and updated features.

In addition, this release includes the following changes that have the potential to change the existing system behavior or interface:

- When searching for resources in the daily view of the schedule board: Once the searched resources are returned, bookings of the resources are not returned on the center area, until the board is refreshed. This bug is now fixed in this update.
- When different capacities are used for a resource before and after a break, (for example 11 AM to 12 PM, working with capacity is 1; 12 PM to 1 PM is a break, and 1 PM to 2 PM, working with capacity 2) then the break time is shown as working time on the schedule board. This bug is fixed in this update. 
- Fixed a bug where quick book is used on a requirement group, and resources work in a different time zone than the time zone of the calendar of the requirements in the group, only a part of the available time slots were returned. With the fix, all available time slots are returned in this scenario.
- Fixed a bug where the search time window of the resource requirement is greater than the time range displayed on the schedule board and schedule assistant, the resource booked hours capacity on the resource cell were not displayed. The expand and collapse button next to the resource in daily, weekly, and monthly views were also not displayed.
- When you enable any entity for scheduling (for example, case, lead, account), enable quick book feature on the booking setup metadata record of this schedulable entity, and set **Disable Requirement Auto Creation for Bookings** to yes. The resource requirement records will not be generated post the creation of the booking record.

## 3.12.29.5 - 2020 wave 2 early access

The release is only applied when an environment is opted into early access and introduces the [resource scheduling 2020 wave 2](/dynamics365-release-plan/2020wave2/service/dynamics365-field-service/planned-features#scheduling) new and updated features.

In addition, this release includes the following changes that have the potential to change the existing system behavior or interface:

- Fixed a bug where a booking rule is used and throws a custom notification on the schedule assistant’s **Create Resource Booking** pane, the **Booking created successfully** was not being displayed. Now with the fix, even when booking rules are defined, the booking creation success notification will be displayed. 
- When a custom date format (for example, dd/mm/yyyy) is used, the booking tooltip's displayed start time and end time are displayed incorrectly. This bug is now fixed. 
- Use openWebResource API to open schedule assistant in the client-side tools like Unified Service Desk, so that no custom actions need to be called to open the schedule assistant. 
- For organizations using Japanese language, in the schedule board’s date picker control now shows the right string in Japanese for the months displayed. 
- For organizations using right-to-left languages like Arabic as their base language, the short weekday names are now displayed on the date picker of the schedule board. Also fixed tooltip positioning issue for different components of the schedule board. 
- Fixed navigation using keyboard tab key on the move bookings to a different Day dialog of the schedule board, to move the focus from the booking statuses picker to the ok button, after a booking status is selected. 
- When a requirement status record is used as a default requirement status in the booking setup metadata record of a schedulable entity, the deletion of the requirement status record will not be restricted. 
- On the schedule board, the fields on the booking tooltip with long strings were truncated. With this fix, the long strings will be word wrapped into a new line. 
- When an open area is selected on the schedule board, a pane opens with a lookup for the resource requirement record. Fixed a bug where the default view on this lookup was not changeable. With this fix, the resource requirement view can be changed to any other active view of the resource requirement entity. 
- On the client extension entity form, the lookup field for the web resource is fixed to show all the WebResource lookup views for CSS, JavaScript, and RESX views. 
- Fixed a bug when requirement groups are used with the work orders; on the schedule assistant, the booking status drop-down on the **Create Resource Booking** pane shows not just the booking statuses of the work order, but also related to other entities. With this fix, the booking status drop-down now only shows the booking statuses of the work order. 
- When a resource requirement record and a bookable resource are selected on the schedule board, and the book button is selected, the **Create Resource Booking** pane opens up with the start and end dates populated based on the requirement selected. When the resource selection is changed, the selected start date and end date are being reset. This bug is now fixed. 
- Improved the tooltip description of the field **Actual Travel Duration** field on the scheduling tab of the bookable resource booking to **Shows the total travel duration. Calculated based on the difference between the Bookable Resource Booking's Start Time and Actual Arrival Time.**
- The edit button on the business closure ribbon is hidden, as this button had no action on the business closure records in the view. 
- Removed unnecessary debug console messages for the business closure entity views. 
- When a new business closure record is created, the duration field is calculated incorrectly by adding an additional day. This bug is now fixed, and the duration field is calculated based on the start time and end time selected. 
- When a requirement status record is created and saved, the requirement status lookup field is read-only, so that this value cannot be changed once the record is saved.
- When a requirement has multiple booking records associated, and one of the booking’s resources is not active, the deactivated resource is filtered, and the uncaught exception is handled. 
- Fixed a bug with the time slot selection on the create resource Booking pane. With this fix, when **Book Based on** setting is set to **Estimated Arrival**, and the user selects a suggested time in the schedule assistant, the time they select is populated as the estimated arrival time in the booking panel. When **Book based on** setting is set to **Start Time**, and the user selects a suggested time in the schedule assistant, the time they select is populated as the start time in the booing panel. 
- Added additional checks on the schedule board default settings to prevent schedule board crash with the **Object reference not set to an instance of an object** error. 
- Fixed a bug where the focus on the resource search control on the weekly view of the list view type of the schedule assistant is lost when typing the resource name.
- The custom date format is now supported on the quick book pane. 
- When a booking is created on the schedule board with duration of zero minutes, **Duration must be greater than 0 minutes** is displayed in English on non-English orgs. This bug is fixed, and the string is now localized.

## 3.12.24.5

- Fixed a bug where the search time window of the resource requirement is greater than the time range displayed on the schedule board and schedule assistant, the resource booked hours capacity on the resource cell were not displayed. The expand and collapse button next to the resource in daily, weekly, and monthly views were also not displayed.

## 3.12.24.4

- When you enable any entity for scheduling (for example, case, lead, account), enable **Quick Book** feature on the **Booking Setup Metadata** record of this schedulable entity, and set **Disable Requirement Auto Creation for Bookings** to yes. The resource requirement records will not be generated post the creation of the booking record. 
- The bug where there are multiple pages of available resources suggested on the schedule assistant, only the resources in the first page set were shown and resources on higher pages were not shown. This bug is fixed, and paging through to next pages, resources will be shown as expected.
- When there are multiple work hours are entered on the same day for a resource (for example, 8 AM to 3:30 PM and 2 PM to 5 PM), there was a bug where the resource work hours calendar was only showing work hours as 2 PM to 5 PM. With this fix, the calendar for the resource would show that the resource is working 8 AM to 5 PM. Also, the same should be reflected on the schedule board. 
- When a resource has working hours (for instance, 9 AM to 5 PM on a day) and has time off 12 PM to 1 PM, there is a bug where schedule board shows that the resource has no working hours on that day, though the time off is for only one hour. This bug is fixed, and with this fix, the resource should show as working from 9 AM to 12 PM and 1 PM to 5 PM on the schedule board. 
- When creating a resource requirement using a work hours template, performance improvements are made to reduce the time of creation for the resource requirement record. 
- When the resource work hours are entered by using non-recurrence patterns for a large number of days, and large number of resources (for instance, more than 2000 resources in the org), when looking for available resources, the schedule assistant takes almost 40 seconds to load resources. Performance improvements are pushed as part of this fix, where in this case, the schedule assistant loads much faster (around five to ten seconds, largely based on the amount of data). 

## 3.12.23.71

- The issue with the filtering on the lookup type fields on the schedule board's requirement panel is fixed. 
- When hovered on the bookings on the schedule board, the tooltip was shown instantly, which sometimes blocked the view or blocked using right-click on the bookings. This issue is now fixed by adding a hover delay. When hovered on the booking, tooltip will be displayed with a delay.

## 3.12.23.27

- The rendering issue for tooltips on bookings of the schedule board is now fixed, by making the tooltip scrollable when the height of the tooltip is larger than the browser size. The hyperlinks on the tooltip can also be selected to open them in a new browser window.
- The text **Hide default requirement panels** is now made visible on the schedule board tab settings under the **Requirement Panels** section, which was previously only partially visible.
- Fixed an issue where entering a comma on the filter control of the filter panel was clearing the input on the filter control. With the fix, the comma will not influence the autocomplete, which was causing issues for customers who have a comma in their filter options.
- If the work hours tab is renamed or removed from a custom bookable resource form, when you select the **Show work hours** button, an error will be displayed: **The Work Hours tab has been renamed or removed from this form. Please update this form to include the Work Hours tab.** Update so that the work hours tab can be added back to the form.
- Fixed an issue on the **Create resource booking** panel on the schedule board. With the fix, the **Start Date** and **End Date** on the panel will always reflect the **From Date** and **To Date** of the requirement selected in the **Requirement Panel** at the bottom of the board.
- The map pins of the resource requirement records are loaded on the map view of the filter panel on the schedule board, based on the view that is defined on **Requirement Map Filter View** on schedule board settings. We fixed the issue where, if the view used here has no filters on the view definition, the map panel never completes loading. With this fix, the map panel would load, regardless of the filters on the view used.
- Fixed an issue where **Universal Resource Scheduling** is used as the scheduling engine; users who are not system administrators were unable to complete the appointment records. With the fix, any user with privileges to complete the appointment record can mark the appointment as complete.

## 3.12.22.9

- For organizations that have [schedule board preview enabled](https://aka.ms/scheduleboard), the schedule board preview can be accessed from **Field Service** application sitemap along with **Universal Resource Scheduling** application sitemap.
- Fixed an issue where booking tooltip blinks when the height of the tooltip is greater than the height of the visible center Gantt area, where bookings are displayed on the schedule board. With this fix, the tooltip would not blink and the user would be able to select the hyperlinks on the tooltip to open the respective record in a new window.
- Fixed the issue where [intervals](/dynamics365/common-scheduler/fulfillment-preferences#interval-setup) functionality of fulfillment preferences was not working on the schedule assistant.
- Resolved the issue of duplicated time slots for the resources on the list view type of the days view of the schedule board.
- Multiple calls to retrieve data in the list view type of the days view are reduced to one call, in order to improve schedule board performance.
- Fixed the issue where available time slots of resources are displayed differently on schedule assistant and the quick scheduling pane for the schedulable entities that do not have an associated resource requirement record.
- The horizontal and vertical view types are now hidden from the requirement group's find availability or schedule assistant screen.
- Fixed the error **The start address and end address cannot be empty**, which is incorrectly thrown on the **Get Driving Directions** functionality on the schedule board, due to an uncaught exception.
- Advanced find on the business closures entity is now supported.
- When using the schedule assistant/find availability functionality, the available time slots should be shown in the same timezone of the requirement calendar; however, if a schedulable entity like case doesn't have a requirement record associated, then the results need to be shown in the timezone of the CRM user preference.
- The issue of resource name truncation in the days view of the schedule board is now fixed.
- Fixed the focus shifting issue on the schedule board, where focus is shifted to a previous booking in focus, when booking status of the bBooking assigned to a resource at the bottom of the resource list. With this fix, the focus would stay on the booking in context.
- Fixed a translation issue on requirement groups in Japanese, where the name of the requirement or subgroups changes from Japanese to English when the record is saved.
- Quick scheduling now supports and handles different date format styles like English (South Africa).  
- Fixed an issue with the **Allow Overlapping** functionality on the bookings. With this fix, when a booking is marked as **Allow Overlapping** set to yes, the schedule assistant (find availability) will show the above booking as an available time slot if the **Allow Overlapping** advanced setting on the filter view is selected.

## 3.12.21.9

- The following Universal resource Scheduling 2020 Wave 1 features in GA and preview planned are included in this release:
  - Next generation schedule board experience (preview)
  - Enhanced work hours calendar for resources
  - requirement dependency for efficient workflow
  - resource scheduling dashboard
- This release also includes all fixes included in the [3.12.9.76 EA package](/dynamics365/field-service/field-service-version-history-resource-scheduling#312976---april-2020-wave-1-early-access).
- Fixed an issue where the booking method on booking panel was not selectable on the list view of the days view in schedule board.
- Fixed a caching issue on the **Get Driving Directions** pop-up functionality of the schedule board, where previously cached values were being used for calculating the route.
- Resolved the incorrect location displayed for the booking on the map view of the schedule board, due to the incorrect formatting issue in conversion of the latitude and longitude on the map in languages like German.
- Fixed the issue where bookings of some schedulable entities cannot be moved to a different day in multiday views like days and weeks views on the schedule board.
- Fixed the issue when a requirement is dragged on to a crew resource on schedule board, a booking is only created for the crew resource and not the underlying active crew resources.
- Fixed an issue where a custom JavaScript is used in the schedule board client extensions to set the default filter values, but the prepopulated default values are only displayed when the respective filter control is selected.
- Fixed an issue where quick scheduling is used on a schedulable entity without associated resource requirement record, and search start and search end dates are passed as the same day; available time slots were displayed for three days rather than one passed in day. With the fix, the available will only be displayed for the date passed in.
- Fixed an issue where booking tooltips are not displayed on hover, when network latency is high.  
- Fixed a null reference exception for booking status metadata checks during the upgrade to improve upgrade experience.

## 3.12.5.13

- resource location can be displayed on the map view of the schedule board's daily view, using the custom entity using the custom geo data settings in the scheduling parameters.
- Fixed the issue with the action msdyn_SearchResourceAvailability was not taking the ConsiderTravelTime parameter into consideration when providing the available time slots.
- Fixed upgrade errors while generating the booking setup metadata records and a few other upgrade improvements.
- Fixed the issue where filters were not saved on the resource utilization view.
- **Booking created Successfully** notification on the schedule assistant is only shown when the booking is created successfully.
- Fixed the incorrect booking time offset on daylight savings time dates for GMT + 1 timezone on the booking and resource requirement forms.
- Fixed null reference issues on the requirement group form.
- Improved error handling on the copy function of the resource requirement form.
- Resource name handling is improved in the search resources lookup on the days view of the schedule board.
- Resource and grid alignment issues are fixed in the hourly view of the schedule board.
- Calendar performance improvements are made for the generation of resource requirements from the project form.
- Improved error handling on the booking rules.
- Schedule board scrolling issues are fixed, when moving the bookings of the resources at the bottom of the list.
- Fixed the issue with the booking tooltip: when there are only two resources displayed on the schedule board, the tooltip masks the booking itself.
- Fixed the issue of the visual duplication of the bookings on the days, weeks, and months views of the schedule board.
- Improved error handling when creating bookings on the schedule board, by adding additional null checks.
- Performance on the schedule board improved by just loading the requirements that are not location agnostic on the map view.
- Fixed the filter panel crash when using the fetch-based filter value and saved as default value.
- Fixed the issue with the schedule assistant filter layout when a filter is changed from multi combo field to non-multi combo filter.
- When **Double book if needed** option is checked on the schedule assistant booking panel, even though the resource does not have enough availability for the requested hours, the resource can be double booked up to 24 hours in one day.

## 3.12.9.76 - April 2020 Wave 1 Early Access

- Fixed a performance issue when upgrading from Field Service version 7.x to version 8.x.  
- Fixed an issue with printing the get driving directions action on the schedule board.  
- When quick scheduling is used to schedule an entity that doesn't have an associated resource requirement, results were always shown in UTC timezone, which is now fixed. The results should always be shown in the user's timezone if there is no requirement calendar.
- Tooltips are now supported on the sort options of the schedule board.  
- A new warning message is now introduced on editing the schedule board settings records: "Modifying these settings has the potential to break the corresponding schedule board tab in a way that cannot be automatically undone".
- Fixed the bug with displaying the resource details in the list view of the schedule board.  
- A new warning message is now supported that the minimum duration needed to create a bookable resource booking is 1 minute.
- The field **Status** is now renamed to **requirement Status** on the requirement status entity.
- Fixed the bug where schedule board crashes when a user record is deleted from the Azure Active Directory, which has an associated bookable resource on the schedule board tab.  
- A select all check box is now supported on the select resources pop-up window on the filter panel sort options.  
- Min rating value now must be less than the max rating value on the rating model entity form.  
- When quick scheduling is enabled on a schedulable entity, the retrieve resources and retrieve constraints queries of the underlying BSM record are called instead of the default queries.  
- Quick scheduling supports the requirement groups with one requirement that has work location type as facility.
- The all/any option labels of the requirement group are now fixed in Danish language.
- Auto apply territory filter field in scheduling parameters form is now deprecated and hidden.  
- Start and end date time fields on the business closures entity form and the grid view are displayed in the same time zones.  
- When a work hours template is applied on multiple resources, a spinner is now added while the work hours are being applied.  
- The from and to date fields on the requirement group form now reflect the timezone from the user's preferences.  
- Details tab on the fulfillment preferences entity form will now only be displayed once.  
- Added a warning on the set work hours template pop-up dialog, that "Applying this work template will overwrite the existing work hours, including time-off".  
- When the map panel on the schedule board is loaded, the map should be zoomed enough to show all the map pins in the requirement map filter view definition.  
- XML syntax validation is now added on editing the schedule assistant filter layout.  

## 3.12.4.9

- Fixed an upgrade issue related to the timezone conversion of the TimeGroupDetail record.  
- Fixed incorrect booking time offset on daylight savings time dates for Auckland timezone.  
- Fixed the issue where some resources show unavailable on the schedule board, due to the number of calendar rules on all the resources on the schedule board.  
- When there are characteristics on the filter panel that are paged, the rating value of the selected characteristic is lost in the filter, which is now fixed.  
- Fixed the flickering issue on the second page of the open requirements tab of the requirement panel.  
- Fixed the alignment of the available time on the days view of the schedule assistant.  
- The filters on the filter panel now support text fields.  

## 3.12.3.9

- The one hour offset issue for the bookings created on the schedule board is fixed in the Brazil daylight savings time.
- The caching issue with the schedule assistant's default availability view setting is set to board is now fixed.
- When a new booking is created on the days view of the schedule board, the board will be refreshed automatically.
- resource requirement map pins are loaded, only when the map view is opened on the filter panel of the schedule board.
- Fixed an upgrade issue due to bad data in the filter values.

## 3.12.2.114

- When the schedule board map view is opened, the map automatically zooms out to show all the map pins.
- The resource lookup is displayed on the schedule board in Arabic.
- On the schedule assistant results list view, work start time aligns with the estimated arrival time values on the create resource booking pane.
- Added additional handling to avoid the corruption of the booking setup metadata and the schedule board settings records.
- Bookings can be edited in the days view of the schedule board by right-clicking on the booking and selecting **Edit**.
- The select resources dialog opens and loads successfully on the filter view of the schedule board, even when there are more than 100 resources enabled to be displayed on the schedule board.  
- When Turkish language is enabled on the org, resource requirement records load under the **Unscheduled Work orders** tab of the requirement pane of the schedule board.
- When double-clicking on the save button the new bookable resource booking form, would not create duplicate records.
- Resources can be searched on the schedule board by their name in the search resources search box.
- map view on the schedule board only shows the pins for the requirements that are returned from the requirement view configured for requirement map filer view setting on the map settings of the schedule board tab settings.
- When Hebrew language is enabled on the org, schedule board loads in the Chrome with browser zoom at 90%.
- The requirement demand pie chart on the schedule assistant information at the bottom is accessible, via screen readers.

## 3.12.1.158

- Workflows can be triggered when resource requirements are created with any allocation method.
- When upgrading URS from version 2.x to version 3.x, resource filters on the schedule board tabs are preserved.

## 3.12.0.448

- Grid alignment issues while scrolling on the schedule board for right-to-left languages (like Hebrew, Arabic) are fixed.
- When a new route is created for a map pin selected on the map panel, the route will stay on top of other routes, even after the auto refresh, which happens when a booking is created or modified.
- On the list view of the schedule board, any linked entity record can be opened by using keyboard, by hitting on the space bar when focused on the linked entity.
- The warning message notification on the schedule assistant is made user-friendly, when Maps are not enabled for a resource requirement when work location is onsite.
- The selected values of the filter "pool type" are also saved along with other filters, when the current filters are saved as default filters.
- When a crew type resource is booked, only the working members of the crew will be booked, crew members, who are not working, will not get booked.
- Custom date fields added to the filter panel as custom filters, will also respect the time zone of the schedule board tab (under Scheduler settings)
- When schedule board settings are opened from the booking setup metadata record of the Schedulable entity, by clicking the Cancel button on the schedule board settings, the form will be closed.
- The scrolling issues on the vertical view of the schedule assistant are fixed.
- On the list view type of days, weeks, and month views of schedule board, the focus will stay on the resource Search box until the typing is complete until focus is moved to a different area of the schedule board.
- The quick scheduling experience will search for available resources in the date range provided in the requirement group and displays available resources on the book resources panel in the date range.
- On successful creation of bookable resource booking record in the offline mode, no unintended warnings will be displayed on the form.
- When looking for a substitute resource on a booking using the "Find Substitution" via schedule assistant, the resource can be substituted on the suggested time slot by clicking on the "Substitute" button, when hovered on the suggested time slot.
- When there are more than 30 suggested resources on the schedule assistant, there will be paging of resources and more suggested resources can be reached by scrolling to the next page.
- When a map pin is selected for a booking on the schedule board, after editing the selected booking, (by dragging and extending the booking), the map pin stays selected.
- Schedule board will support booking alerts are in large number (~200).
- Only active booking statuses will be displayed on the booking status dropdown field on the booking panel of schedule board, when creating bookings.
- When searching for available resources for a requirement group, suggested resources will always be shown in list view only.
- Resources on the schedule board tab can be selected via Select resources under the filter Options on the Internet Explorer Version 11.
- When calling the msdyn_SearchResourceAvailability action using a requirement with a fulfillment preference for time group as input, the output time slot of the action will contain valid TimeGroupDetails.
- Bookable resource bookings can be created on the daylight saving days (entering and exiting daylight savings time).

### Enhancements

- Accessibility improvements are made on the schedule board and schedule assistant.

## 3.11.0.421

- Columns in the list view of the schedule board resize based on the size of the browser (Internet Explorer)
- A few accessibility issues on the schedule board and quick scheduling panel are fixed.
- Days/weeks/month views on the schedule board support the bookings for the schedulable entities without resource requirements.
- When viewing the bookings of requirement group in Split view, the bookings in the Split view will be shown in the same timeline as of the requirement group bookings in the top half of the grid.
- work hours of a resource with capacity greater than 1 in a day, will reflect on the schedule board accordingly.
- Resource capacity booked percentage reflects the resource's bookings in the days, weeks, and month views of the schedule assistant.
- The focus remains on the selected date when a resource is selected from the resource dropdown filter after selecting a date on the calendar of the quick scheduling panel.
- When a resource requirement with a characteristic and rating is booked, the characteristic filter will be populated with the characteristic and rating value from the resource requirement in the filter view of the schedule assistant.
- The search start/search end and time from promised/time to promised date time filters on the filter view of the schedule assistant reflect the from date/to date and time from promised/time to promised from the resource requirement records.
- The membership of the members of a crew type resource on the schedule board is shown in the timezone of the schedule board.
- Only one resource can be selected from the recommended resources on the list view of the schedule assistant.
- When searching for available resources for an onsite requirement group, and a suggested time slot is selected, the estimated arrival time and start fields in the create resource booking panel are filled with the start time and travel start time values from the list view.
- When hovered on the bookings on the schedule board, booking card is displayed with a delay.
- A booking can be created for a work order in the days, weeks, or month views of the schedule assistant.
- Schedule board loads bookings of resources, even with resources who have no calendar or have multiple calendars.
- Rebook for bookings would work even with null values of the filters passed to the schedule assistant.
- The schedule board and schedule assistant will load booking and resource availability on the Internet Explorer Version 11.

### Enhancements

- Support for preferred and mandatory resource in finding available resources.
- Usability improvements to the facility search scenarios via quick scheduling experience.

## 3.10.0.239

- Only valid hex characters can be entered on the status color field on booking status form.
- The overlapping bookings in the vertical view of the schedule board are separated by 1-px spacing.
- Non-working hours color name is consistent across the schedule board tab settings and the schedule board settings configuration record.
- Long names will be wrapped inside the booking tooltip.
- Deletion of a resource is not allowed if it has any group memberships active or inactive, parent, or child, has any associations active or inactive, resource 1 or resource 2.
- When default sorting is added to the schedule assistant retrieve constraints UFX query in the default schedule board settings, the sort by filter of the schedule assistant is pre-filled with the field by which sorting is done and the returned resources are sorted accordingly.
- A few accessibility issues on the schedule board are fixed.
- Schedule board to load the resources in days, weeks, and month views with resources having a valid calendar and wouldn't fatally fail if a resource has an invalid calendar.
- Combo control filter with multiset to false, the selected value will show in the filter.
- Active resource requirements view is sorted on created on by descending order.
- Derive capacity from group members field on the pool resource form can be set to yes or no as required.
- Search resources can be used to search resources in the suggested resources in the list view of the schedule assistant.
- Custom booking template with fields from linked entities of bookings is supported.
- Resource type filter on the schedule assistant will not remember the previously selected values, once unselected.
- The schedule assistant loads as expected when clicked on book button on a work order form in Arabic.
- When a booking is created by schedule assistant, the booking method field on the booking form is populated as schedule assistant.

## 3.9.0.42

- The filter is not enabled for the owner column on the unscheduled work orders requirements view in the requirement grid of the schedule board.
- The refresh button on the requirement grid is disabled while the grid is refreshing the data.
- Alignment for resource icons and the zoom slider on the schedule board are fixed for Arabic language.
- When searching for resources in one view like horizontal, when switched to another view, like list view, the search is still retained along with the search text and results.
- The bookings can be moved to a different time or resource by dragging and dropping the booking on days, weeks, and month views of the schedule board.
- Quick scheduling would be using the "As The Crow Flies" approximations to calculate travel time if Bing maps integration is not enabled.
- Improved error messaging on the schedule assistant when looking for available resources and on the schedule board when displaying the bookings.
- When auto update booking travel is enabled, and onsite bookings are created by the quick scheduling, the travel time to the subsequent bookings is updated based on the location of the previous booking.
- The schedule assistant search for available resources will be successful with continuous multiple associations on a single day for a resource type facility.
- When an onsite requirement is selected in the requirement grid, the location pin is selected and focused in the map view. Once clicked on "Find Availability," the location pin on the map view will stay selected entering and exiting the schedule assistant.
- Alignment of the fields on the fulfillment preferences form is fixed.
- Alignment of the sort arrows on the sort options control on the schedule board is fixed.
- Time out issues request to msdyn_RetrieveResourceAvailability is posted from a web app are fixed.

### Enhancements

- FetchXML query is replaced by query expression for the action that fetches work order bookings to improve the performance.

## 3.8.0.105

- The date selector on the schedule assistant list view is dimmed because it has no effect on the resources displayed when searching for availability of a requirement or a work order.
- When booking a schedulable entity record, only the booking status that is mapped to the booking status field logical name of the booking setup metadata record of the schedulable entity will be on the schedule assistant. For example, when scheduling a work order, only the option set values of the field msdyn_fieldservicestatus will be displayed in the booking status drop-down on the schedule assistant,
- When searching for availability of resources on a requirement, the number of matching resources returned in the search on the schedule assistant is limited to the value set on the field resource availability retrieval limit on the default metadata settings of the booking setup metadata record. The default value of resource availability retrieval limit is 100.
- Only one booking setup metadata for an entity can be created.
- For German locale, on the schedule assistant, remaining duration does not overlap with the pie chart visual next to it.
- Only Active resources can be added to a resource pool or resource crew's children.
- A few accessibility issues on the schedule board are fixed.
- The resource requirement form can be customized to remove optional fields like resource type from the form.
- Selected sort on the schedule board is determined by the Sort result by filter on filters.
- The booking alerts template field on the default schedule board settings shows the default HTML template value.
- **Book** and **Book & Exit** buttons on the schedule assistant are enabled only when at least one eligible resource is returned on the schedule assistant.
- Multiple characteristics can be selected on the filters on the schedule board.
- A booking cannot be deleted when it has an associated booking alert.
- When booking a requirement in the weekly view or monthly view of the schedule assistant, if the availability search start date is today and is not the first day of the week or month, the start date will correctly default to today, so that the book button is enabled.
- The work location filter on the schedule assistant will show all three possible values: onsite, facility, and location agnostic.
- The filters on the schedule board will show the right values in the drop-down even when the user manually types in the filter.
- When Auto Update booking travel is enabled in the scheduling parameters, travel time of the adjacent bookings is updated when a booking is created in the list view of the schedule assistant.
- Correct search results are displayed on the quick scheduling panel for all timezone values set on the resource requirement form.
- A multi resource work order, that is, a work order associated with a requirement group, can be booked via quick scheduling.
- Requirement group bookings can be viewed in split view.
- The Timeline header on the schedule board will be shown even after exiting the schedule assistant by selecting exit search.
- The rating values on the rating model form are ordered by rating values, not the names.
- The resource card can be opened by right-clicking the resource, even when the resource has characteristics with no rating values.
- When booking a requirement group via the schedule assistant, selecting a time slot on the list view opens up the Create resource booking Panel on all browsers.
- When booking a requirement group or the requirements under that requirement group, the same results are displayed on the schedule assistant.
- Facility requirements can be booked via quick scheduling with the correct duration of the booking.
- You can book work orders on the days view of the schedule assistant.
- Multiple issues preventing upgrade.

### Enhancements

- Performance improvements to schedule board refresh times when multiple crew type resources are present on the schedule board.
- Performance improvements to searching for resource availability for requirement Groups.
- Reduced unnecessary calls to retrieve the resource requirements name and booking setup metadata. Other duplicated calls are also reduced when searching for availability.
- Self-service scheduling API is now available to schedule the single resource requirement, with a corrected process name **Resource Scheduling – Search Resource Availability** and unique name msdyn_searchresourceavailability.
- From and to date fields on the resource requirement entity are restricted to have only the User Local behavior to avoid Time Zone functionality loss on the schedule assistant and loss of the time zone data on resource requirements.
- Added a suggestion to service health diagnostics to show the suggestion/fix with manual steps when resource booking sync job is disabled but the feature synchronize resource bookings with outlook is enabled.
- When using URS on Unified Service Desk, the schedule board can be loaded without having to pass the full Unified Interface context.
- Quick scheduling now supports scheduling of onsite requirements.

## 3.7.0.70

- Requirement group control loads in the service form on the customer service scheduling app.
- When a schedulable entity without a resource requirement is booked via the schedule assistant (pop-out schedule board) days, weeks, or months views, the booking status is populated to the default status.
- The resource routes are optimized by listing using the schedule board driving directions in the sort order of a booking's start time.
- Optimized rebooking in the schedule board by fixing a client-side console error.
- Map view icon is no longer displayed in the schedule assistant view.
- Changes on the default schedule board settings form are saved when accessed from booking setup metadata record.
- Drag and drop the bookings from one resource to another or from one time to another of the same resource in days, weeks, or months views.
- Resource names with apostrophes, like O'Brien, can be searched on the schedule board resources.
- Booking a resource requirement for the facility resource type now populates the resource filter field as a facility in the schedule assistant (pop-out schedule board).
- Book based on setting for the schedule board shows how the time slot suggestions are displayed in the Hourly view of the schedule assistant, and more details on how to use book based on are included.
- Duration filter on the schedule assistant for Hebrew is fixed when the value of the duration is 1.
- Travel start time on the schedule assistant list view shows as travel time subtracted from the work start time.
- Drag and drop multiple open requirements to an expanded resource in days, weeks, or months view to create multiple bookings.
- Rendering of the resources on the schedule board is improved.
- View resource cards in the schedule assistant for requirement groups availability.
- Schedule assistant minimizes the number of resources necessary to fulfill a requirement group when the Sort result by field is set to Fewest resources first.
- Multiple issues preventing upgrade.
- Drag resource route on the map to a requirement pin to create a booking for the resource.
- The Select resources filter can be used to select the resources to be displayed on the schedule board.
- Only active members of the crew with valid crew membership will be booked when a crew is booked.
- Driving directions and the map view on the schedule board have the same traffic icon.
- The position of the hover book button on the suggested time slots is adjusted when the preceding booking is extended beyond the suggested time slot.
- When a requirement is selected and the requirements panel is refreshed, the requirement selection persists.

### Enhancements

- Made improvements to uptake new endpoint Bing distance matrix APIs.
- Self-service scheduling API is now available to schedule the single resource requirement.
- The work location for new requirements added to a requirement group is now inherited from the work location of the existing requirements in the requirement group, and is kept in sync.
- The calendars of the requirements of a requirement group are kept in sync and share the same calendar. Changing a calendar or time zone for one requirement updates it for all the requirements of the requirement group.
- When booking a requirement group, the schedule assistant is launched in the time zone of the requirement group's requirements because they all share the same requirement.
- Performance improvements to searching for resource availability, viewing bookings on the schedule board, creating bookings for crews, creating bookings in the hourly views of the schedule board, and when using other URS plug-ins.

## 3.6.0.18

- On the schedule assistant, the radius unit behavior reflects kilometers or miles as per the preferred unit of distance when "Search for" field is changed.  
- The zoom level on the "Map View" on the "Filter Panel" will be preserved after entering or exiting the Schedule assistant search. 
- Only activated members of a crew get booked when a crew is booked.
- On the schedule board setting for schedule assistant, the unavailable resources field can be changed from "Unavailable resources do not appear" to "Unavailable resources appear dimmed" to show the unavailable resources on the schedule assistant.
- Alignment of scheduler settings controls.  
- On a schedule assistant search for available resources on a location agnostic resource requirement, the "Time From Promised" and "Time to Promised" time window precedes over the "Search Start" and "Search End" time window, and the recommendations will be presented to make sure the technician can start work in the "Time From Promised" and "Time To Promised" window.
- Onsite multi-resource requirements will be presented with travel time in the schedule assistant recommendations.
- The filter panel's characteristic field on the schedule assistant is populated with the characteristic from the resource requirement or work order.
- Multiple issues preventing upgrade.
- Resource utilization of a resource on non-working day, along with the color code of the non-working day.
- Dragging the technician travel route to a requirement pin to schedule the booking in the maps view on the filter panel of schedule board.
- The schedule board setting "Order Number" default maximum value is increased to 1000 from 100.
- Duration field value text in Hebrew on schedule assistant.

### Enhancements

- When inserting a booking between two bookings or reassigning a booking to another resource, the travel time of all associated bookings will be recalculated and updated on hourly schedule board and schedule assistant. This feature can be enabled by "Auto Update booking travel" field under **Resource Scheduling** > **Settings** > **Administration** > **Scheduling Parameters**.
- When the **Book** button is used on the resource requirement and the timezone on the pop-out schedule board is updated, the date time fields on the bottom requirement info panel will reflect the changed timezone.
- All the date and times in the filter panel and requirements panel on the schedule board are updated when the time zone is changed in the scheduler settings on the schedule board.
- Various performance improvements when searching for resource availability.

## 3.5.0.107

- Booking status on the create resource booking panel is always defaulted to either front load or the last used value on the schedule board.
- On the schedule assistant, a new booking can be created in custom time, by clicking and dragging in the demand panel, which opens the create resource booking panel for confirmation of booking details.
- A resource requirement record can be created by quick create forms on the schedule board, even there are no resources on the schedule board tab are working.
- When the start and end locations of the bookable resource are set to organizational unit address, the organizational unit field becomes mandatory field.
- The row height and column width slider tooltip value is now localized.
- The location of the tooltip, when dragging and dropping an existing booking on the board is corrected in the Hebrew language orgs.
- Slider controls on the scheduler settings of the schedule board are aligned in the orgs with right-to-left languages.
- Error handling improvements on the schedule board.
- Resource requirement details associated view of resource requirements includes additional details like duration, from and to fields.
- The skills subgrid in the resource requirement form will only show relevant data and hide the redundant data like the resource requirement name field.
- On the schedule board, bookings can be created with the start/end dates in the past.
- Contains solution upgrade improvements.
- Select resources dialog opens for selection of resources to be shown under the schedule board tab
- The working time of the schedule board tab can be configured by using the start time and end time slider controls under the scheduler settings of the schedule board tab.
- Duplicate booking creation on the schedule board, due to network race conditions is now fixed.
- The availability cells in the days view of the schedule board are appropriately aligned on the daylight savings days at 12:00 AM.
- The duration of the bookings on the multi-day views of the schedule board can be decreased by dragging the right end of the booking to left or left end of the booking to right.
- The pre-filled characteristic-Rating value in the filter view, can be selected to view it the filter view.
- Booking rules dialog respects the cancel button and wouldn't create a booking.
- When looking for available resources using a resource requirement for resource type facility, in the list view of the schedule assistant, organizational unit column shows the appropriate string values.
- When clicked on maintain bookings for a team member, opens up the schedule board with the project bookings for the selected team member.
- Book button is displayed on the resource requirement form for the users only with appropriate read/write privileges to the entity.
- Resource requirement for facility type pool can be searched for available resources using the schedule assistant or find availability.

### Enhancements

- Improvements are made to the date time controls by leveraging the Office fabric UI control on the resource requirement, fulfillment preferences, and time group detail forms.
- Scheduling Health Diagnostics provides capabilities to detect and suggest self-healing options with regard to:
  - Unsupported customizations on internal use only web resources.
  - Actions and workflows that are in draft state.
  - Essential SDK message processing rules that are in disabled state.
  - Missing metadata records such as booking setup metadata records, default UFX query values.
- Improvements are made to the icons on the booking right-click menu.
- If **Connect to Maps** is disabled, the travel times will be calculated based on the "Crow fly" approximations.
- Performance improvements for the retrieve resource availability action calls on the multi-resource requirements with fulfillment preferences (intervals).

## 3.4.0.141

- Custom date and time fields now display properly on schedule board panels.
- Issues opening and saving schedule board resource picker under options in filter control.
- Paging issues when using schedule board resource picker under options in the filter panel.
- When "Time From Promised" on the requirement is in the past and you search for availability, the value is now moved to the current time and the search button is enabled.
- Changing the schedule board working time no longer immediately closes the settings dropdown.
- Book button now appears on views and forms when using USD.
- Resources associated to a facility with a parent Organization Unit that is different from the associated facility correctly use facility organizational unit when it comes to schedule assistant facility search.
- Miles/kilometers default properly from scheduling parameters entity.
- Generic resource type is removed from resource picker under the select resources dialog.
- Auto focus on characteristic rating value in filter control when entering schedule assistant on certain devices.
- Overbooked requirements no longer show a negative duration in booking panel when in schedule assistant
- Facility searched properly group results by organizational unit, regardless of the value in the "part of same" field on the requirement group control.
- Resources that are location agnostic, yet are associated to a facility, will return in facility searches for the time they are associated to the facility.
- Issue selecting pool type on schedule board filter panel while using Firefox browser.
- Selecting cells in daily, weekly, and monthly boards while in schedule assistant now passes information to the booking panel properly.
- Schedule boards that have characteristics with rating values saved no longer prompt user to enter a rating value.
- Issue on certain devices where current timeline bar on schedule board wasn't showing correct time.
- Work location on booking is now set properly when using drag and drop on schedule board.
- Misaligned labels for languages that read right to left.
- Issue loading schedule board in Internet Explorer 11.
- Issue creating schedule alerts from certain places.

### Enhancements

- Various performance improvements when creating bookings.
- Dragging to extend a booking on multi-day schedule boards opens booking panel instead of booking dialog.

## 3.2.0.405

- If a booking has the work location field set to location agnostic, the booking will be treated as location agnostic even if there is a latitude and longitude value on the booking.
- Issue with schedule board list view refreshing when changing between hourly and daily.
- When searching for a resource in the resource search bar on the schedule board list view, if no resources can be found, the board properly removes all resources.
- Issue dragging a requirement from the map to the schedule board while using Firefox browser.
- Changing "derive capacity" field on a pool resource from no to yes now triggers the calendar to be calculated based on the child resources of the pool.
- Issues when changing between horizontal and vertical schedule board while in split view.
- Issue loading schedule board with many explicitly saved resources.
- Resource's location is now properly taken from the facility it is associated to.
- When using a language that reads from right to left, the resource name is now properly rendered on the schedule board.
- When launching the schedule assistant from a schedulable entity, the user now lands back on the same form after clicking book and exit.
- Schedule board no longer shows resource with a capacity greater than 1 as available all day.
- When booking a requirement group using the schedule assistant, the booking status dropdown now properly filters to the booking statuses for that schedulable entity.
- Issues loading requirement group control in the Microsoft Edge browser.
- When using the schedule assistant to schedule a requirement group for a facility, there is no longer a travel time conflict between the facility and the resources.
- Double booking option in schedule assistant on daily, weekly, and monthly boards now properly books the resource even if the resource has no remaining capacity.
- Appointment schedule board settings are now generated properly.
- Issues in certain scenarios where schedule board had issues loading in Internet Explorer.
- "Supplied DateTime represents an invalid time" error.
- Error message when scheduling a single requirement to a crew resource.

### Enhancements

- Resources associated to facilities will no longer return in onsite schedule assistant searches. This prevents customers from accidentally scheduling a resource that should be stationed at a facility from going to a customer location.
- Resources that are not associated or related to a facility will no longer return in facility searches. Currently, when a resource is set up to work at a facility through an association or as a child resource of a pool, URS does not account for travel to the facility.
- When using the schedule assistant to schedule a requirement group, if the requirement's work location is set to facility, and there are no options selected under the "part of same" attribute, the search will execute as if part of same "resource Tree" is selected.
- Saving a filter on the schedule board now shows a green confirmation check mark instead of a yellow warning symbol.
- Warning message will now be displayed when trying to change the latitude or longitude field on a booking.
- Added validation to check that if a resource is associated to a facility, then it should not be allowed to be a child resource of a pool associated to a facility or facility pool for the same time frame.

## 3.1.0.166

- If a booking has the work location field set to location agnostic, the booking will be treated as location agnostic even if there is a latitude and longitude value on the booking.
- Issue with schedule board list view refreshing when changing between hourly and daily.
- When searching for a resource in the resource search bar on the schedule board list view, if no resources can be found, the board properly removes all resources.
- Issue dragging a requirement from the map to the schedule board while using Firefox browser.
- Changing "derive capacity" field on a pool resource from no to yes now triggers the calendar to be calculated based on the child resources of the pool.
- Issues when changing between horizontal and vertical schedule board while in split view.
- Issue loading schedule board with many explicitly saved resources.
- resources location is now properly taken from the facility it is associated to.
- When using a language that reads from right to left, the resource name is now properly rendered on the schedule board.
- When launching the schedule assistant from a schedulable entity, the user now lands back on the same form after clicking book and exit.
- Schedule board no longer shows resource with a capacity greater than 1 as available all day.
- When booking a requirement group using the schedule assistant, the booking status dropdown now properly filters to the booking statuses for that schedulable entity.
- Issues loading requirement group control in the Microsoft Edge browser
- When using the schedule assistant to schedule a requirement group for a facility, there is no longer a conflict of travel time between the facility and the resources.
- Double booking option in schedule assistant on daily, weekly, and monthly boards now properly books the resource even if the resource does not have any remaining capacity.
- Appointment schedule board settings are now generated properly.
- Issues in certain scenarios where schedule board had issues loading in Internet Explorer.
- "Supplied DateTime represents an invalid time" error.
- Error message when scheduling a single requirement to a crew resource.

### Enhancements

- Resources associated to facilities will no longer return in onsite schedule assistant searches. This prevents customers from accidentally scheduling a resource that should be stationed at a facility from going to a customer location.
- Resources that are not associated or related to a facility will no longer return in facility searches. Currently, when a resource is set up to work at a facility through an association or as a child resource of a pool, URS does not account for travel to the facility. Therefore, only resources set to work at a facility will return in facility searches.
- When using the schedule assistant to schedule a requirement group, if the requirement's work location is set to facility, and there are no options selected under "part of same" attribute, the search will execute as if part of same "Resource Tree" is selected.
- Saving a filter on the schedule board now shows a green confirmation check mark instead of a yellow warning symbol.
- Warning message will now be displayed to a user if they try to change the latitude or longitude field on a booking.
- Added validation to check if a resource is associated to a facility then it should not be allowed to be a child resource of a pool that is associated to a facility or facility pool for the same time frame.

## 2.4.11.59

[Read a blog post about the bug fixes](https://cloudblogs.microsoft.com/dynamics365/it/2019/05/14/enhancements-and-bug-fixes-in-universal-resource-scheduling-urs-version-2-4-11-59/).

## 2.4.10.56

[Read a blog post about the bug fixes](https://cloudblogs.microsoft.com/dynamics365/it/2019/05/01/release-notes-for-universal-resource-scheduling-version-2-4-10-56/).

## 2.1

[Read a blog post about the bug fixes](https://cloudblogs.microsoft.com/dynamics365/it/2017/05/19/universal-resource-scheduling-solution-for-dynamics-365-update-6-1/).
