# local-Storage & session-Storage & Cookies
Local Storage,  Session Storage and Cookies all extend storage and all are used to store data on the client side. Each one has its own storage and expiration limit.


# local-Storage
The data stored in local-storage persists until explicitly deleted. Changes made are saved and available for all current and future visits to the site.
stores data with no expiration data,and gets cleared only through JavaScript, or clearing the Browser Cashe / Locally Stored Data.

# session-Storage

Changes are only available per window. Changes made are saved and available for the current page, as well as future visits to the site on the same window. Once the window is closed, the storage is deleted.

# Cookies
stores data that has to be sent back to the server with subsequent requests. Its expiration varies based on the type and the expiration duration

Cookies => server-side || client-side . normally from server-side .
localStorage && sessionStorage read => client-side.

# The difference ??

localStorage is similar to sessionStorage, except that while data stored in localStorage has no expiration time, data stored in sessionStorage gets cleared when the page session ends — that is, when the page is closed.

# Why would you use cookies vs local/session storage?
localStorage and sessionStorage are perfect for persisting non-sensitive data needed within client scripts between pages, for example: preferences, scores in games.

Cookies are used for authentication purposes and persistence of user data, all cookies valid for a page are sent from the browser to the server for every request to the same domain - this includes the original page request , all images, style-sheets, scripts and fonts .cookies can be made secure by setting the httpOnly flag as true for that cookie. This prevents client-side access to that cookie
