# Non-functional Requirements

- It's not estimated the number of shows and seat reservations daily yet.

- Past reservation data (fk) can be deleted. No programmatically generated user data.

- Strong consistency for bookings, or more precisely listing availability, so there will be no double bookings or bookings on unavailable dates in general.

- High availability because there are monetary consequences of lost bookings.

- High performance is unnecessary. P99 of a few seconds is acceptable.

- Typical security and privacy requirements. Authentication/Authorization required. User data is private. 

