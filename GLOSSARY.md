# WeighIn

The language for recording and reviewing one person's weight and user-defined body measurements over time.

## Language

**Measurement Type**:
A distinct body measurement tracked over time. Weight is built in; custom measurement types are named body lengths such as Waist or Left Bicep.
_Avoid_: Custom unit, metric

**Measurement Entry**:
The measurement values belonging to one user and one measurement date. An entry contains at least one value and no more than one value per measurement type.
_Avoid_: Daily log, submission

**Measurement Value**:
A single weight or body-length quantity associated with a measurement type and measurement date.
_Avoid_: Reading, statistic

**Active Measurement Type**:
A custom measurement type available for new measurement values.
_Avoid_: Current measurement

**Archived Measurement Type**:
A custom measurement type withheld from new entries while its history remains available. It can be restored to an active measurement type.
_Avoid_: Deleted measurement

**Measurement Date**:
The user's local calendar day to which a measurement entry belongs, rather than the moment its data was saved.
_Avoid_: Timestamp, creation date

**Measurement Template**:
An optional predefined custom measurement type offered during initial setup.
_Avoid_: Default measurement

**Unit Preference**:
A user's account-wide choice between metric and imperial units for displaying weight and body lengths.
_Avoid_: Measurement type, custom unit

**Measurement History**:
The chronological collection of a user's measurement entries, reviewed as a list or as a trend chart for one measurement type at a time.
_Avoid_: Activity feed
