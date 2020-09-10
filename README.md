## Webbeds outgoing IP ranges

This document contains the list of IP ranges in use from Webbeds platforms to connect to external suppliers. It is presented in 
[json format](ranges.json).

### Recomendations

This list is dynamic so it can change at any moment, adding, modifying or deleting ranges. Please consider to access this file periodically  to keep it up to date.

In case you can automate this reading, which is something we recommendd, you can use the fields `syncToken` or `createDate` to check if file has changed.

### Format of the file

 * `syncToken`: It will change with each update. You can use it to control if the file has changed or not.
 * `createDate`: The date of the last update of the file. You can use it too to control if the file has changed or not.
 * `prefixes`: List of all the IP ranges
   * `ip_prefix`: IP range that should be considered as from WebBeds. It uses [CIDR Notation](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing#CIDR_notation).
   * `region`: Ignore (For internal use of WebBeds)
   * `brand`: Ignore (For internal use of WebBeds)
   * `dc`: Ignore (For internal use of WebBeds)
