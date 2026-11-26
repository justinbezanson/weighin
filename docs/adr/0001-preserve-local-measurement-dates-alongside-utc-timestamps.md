# Preserve local measurement dates alongside UTC timestamps

We store each entry's local measurement date and IANA timezone alongside UTC record timestamps because a UTC instant alone cannot preserve the original measurement day after a user changes timezones. Daily uniqueness and history grouping use the stored measurement date, while any displayed record timestamp is converted to the user's timezone. This avoids inventing a time of day for date-only or backfilled measurements without allowing later timezone changes to move historical entries to another day.
