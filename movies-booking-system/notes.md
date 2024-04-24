# Notes

## Not to use an in-memory cache
In search results, we only display available movies. If a movie is highly desirable, it will soon be reserved and no longer displayed in searches. If a movie keeps being displayed in searches, it is likely to be undesirable, and we may choose not to incur the costs and additional complexity of providing a cache. 

Another way of stating this is that cache freshness is difficult to maintain, and the cached data quickly becomes stale.

## Handling overlapping bookings

If multiple users attempt to book the same seat with overlapping shows, the first user’s booking should be granted, and our UI should inform the other users that this seat is no longer available for the shows they selected and guide them through finding another available room.

## Lock seats during booking flow

When a user clicks on a search result to view the details of a room and possibly submit a booking request, We can lock these seats in for the show in a few minutes. During this time, searches by other users with overlapping shows will see the seat lock status.

If this seat is locked after other users have already received their search results, clicking on the seat should present a notification of the lock.