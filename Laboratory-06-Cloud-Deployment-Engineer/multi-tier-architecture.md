# Two-Tier Architecture

A two-tier architecture splits an application into two layers: one that users interact with and one that stores data. The two layers communicate over a network. In this lab, the two tiers are Nextcloud (application) and MariaDB (database).

## The Web/Application Tier

The web/application tier runs Nextcloud. It serves the user interface in the browser, handles HTTP requests from users, and runs the application logic such as logins, file uploads, and file sharing. Whenever it needs to read or save information, it sends a request to the database tier.

## The Database Tier

The database tier runs MariaDB. Its role is to store persistent data such as user accounts, credentials, and file metadata. It only receives queries from the application tier, and users never connect to it directly.

## Why Separate Them?

Separating the web server and the database into two containers lets each one be updated, restarted, or fixed without affecting the other. It also allows each tier to be scaled independently and keeps the database hidden from the public, which improves security. If something breaks, it is easier to find which container is the problem.
