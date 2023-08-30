![Visitor Count](https://profile-counter.glitch.me/amwalding5/count.svg)
# IPv6 Extension Header PCAPs

For those who know networking, there are very few opportunities to get your hands on packet capture (pcaps) that have IPv6 Extension Headers.  There are a number of reasons for this, and one is that extension headers in IPv6 have always been a security vulnerability.  So many service providers do not support transport of IPv6 packets with extension headers.
* Initial Tests in 2014 were recorded in RFC 7872 https://www.rfc-editor.org/rfc/rfc7872
* Geoff Huston has set up a worldwide testing client/server system that tests this worldwide: https://stats.labs.apnic.net/v6frag

## What are IPv6 Extension Headers?
* Extension headers fit between the IPv6 header and the Layer 4 headers (UDP or TCP)
* Note: IPv4 supports this capability, but has never been utilized
* IPv6 header is fixed to 40 bytes, so extensions allow features to be added beyond this limit
* Extension Headers are part of the Payload
* Primarily end-to-end – not processed by intermediate nodes
* Extension Headers are designed to make IPv6 extensible to add features we may not even contemplate today.

## Are Extension Headers Supported in Limited Domains?
* Limited Domains are domains that are 
  * Managed by a single entity – think a company, a university, perhaps a provider
  * A network that is firewalled off the larger network
* Enterprise Networks (generally) have been hesitant to deploy IPv6
  * Security issues (privacy of extension headers), other “gaps”
  * Can extension headers support segment routing, OAM, other features?
  * Enterprises need to understand the exact use cases
* Some Universities report free flow of Extension Headers inside their networks, but policing at the network edges
* Possible use cases: 
  * Some kind of Traffic Engineering
  * Using IPv6 as an underlay network?

I searched and searched and could not find a good source of IPv6 extension header samples. So I have created this repository to try to provide some for researchers/engineers.

Here are a collection of IPv6 Extension Header packet captures for those interested in what they look like in Wireshark.

That said, if you are a researcher like me I hope this little repository helps.  You may also want to grab my IPv6 Wireshark Profiles from that repository.

If you want to contribute - please let me know.

You can find more Wireshark related stuff here in Github (like my profiles repository) and here: https://www.cellstream.com/tag/wireshark/ - at my web site.
Also, feel free to browse our other IPv6 related articles and information here: https://www.cellstream.com/tag/ipv6/

Did I just save you time and $$$? I certainly hope so. Return the favor - buy me a coffee: https://www.buymeacoffee.com/awalding or become a patron: https://www.patreon.com/bePatron?u=22427713&redirect_uri=https%3A%2F%2Fwww.cellstream.com%2Fcomponent%2Ftags%2Ftag%2Fwireshark&utm_medium=widget

Thanks for supporting my work.
