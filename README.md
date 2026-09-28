# BookMyShow Style Seat Booking Demo

## Run
1. Extract the ZIP file.
2. Open `index.html` in a browser.
3. Select available seats.
4. Click "Book Tickets".
5. Click "Close Window" after the booking succeeds.

## Important browser behavior
JavaScript cannot reliably close a normal browser tab/window that the user opened directly.
`window.close()` normally works when the page was opened by JavaScript, for example:

```javascript
const bookingWindow = window.open("index.html", "_blank");
```

For a real booking application, replace the demo booking section in `script.js`
with an API call to your backend/database before displaying the success message.

This demo does not process real payments or create real bookings.
