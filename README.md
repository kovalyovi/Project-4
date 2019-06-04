# How to successfully run the application

1. The `allFeeds` variable must contain objects with both `url` and `name` properties set up which must be defined.
2. The `body` must have `menu-hidden` attribute by default which will hide the show-menu.
3. Clicking on the `menu-icon-link` reference tag must toggle the `menu-hidden` class of the `body`
4. Function `loadFeed` must accept two arguments: `id` and `callback` function to run at the end of the receiving of the `success` and in the `reject` parts of the request.
After making the request and receiving the response, it must have at least one entity with the class `.entry`.
5. Switching topics under `menu-icon-link` must call function `loadFeed` and pass two arguments - `id` and `callback`. 
Different `id`'s must provide at least one response from the server which must be different from each other.
