<hr class="core" style="display:none"/>
<h2>Core Context Management</h2>

If you want your application to be “smart”, you have to first make it “aware”.
FIWARE provides you with means to produce, gather, publish and consume context
information at large scale and exploit it to transform your application into a
truly smart application.

Context information is represented through values assigned to attributes that
characterize those entities relevant to your application.
[The Context Broker GE (open source reference implementation: Orion)](https://fiware-orion.readthedocs.io/en/master/)
is able to handle context information at large scale by implementing standard
REST APIs.

[![1](images/1.png)](images/1.png) Context information may come from many
different sources:

-   Already existing systems
-   Users, through mobile apps
-   Sensor networks

One of the most important features of the Context Broker GE is that it allows to
model and gain access to context information in a way that is independent from
the source of that information. As an example, your application may need to be
aware about “Places” (identified by their specific geographical coordinates) and
the “temperature” in them.  The way in which the temperature of a given place is
obtained may vary from place to place.  Thus, the temperature of a given street
may be measured through temperature sensors deployed in that street, while in
another street it may be obtained through temperature sensors deployed on buses
that circulate through the street and even in some other streets may be obtained
through users who report the temperature using their mobile phones.  Using the
RESTAPI exported by the Context Broker GE, the way in which your application
will be able to query the temperature of places, or subscribe to changes on
temperatures of places will be the same no matter which is the source of a
temperature and it will not vary if the source of the temperature for a given
place changes over time (e.g., the temperature of a given street turns to be
measured through temperature sensors deployed on the streets rather than through
buses equipped with sensors).

[![2](images/2.png)](images/2.png)

## What is FIWARE? - Introductory Presentations

Presentations about FIWARE from recent FIWARE Global Summits:

| Porto 2018                                                                                 | Malaga 2017                                                                                                                   |
| ------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------- |
| [FIWARE Overview](https://www.slideshare.net/FI-WARE/fiware-global-summit-fiware-overview) | [FIWARE Overview](https://www.slideshare.net/FI-WARE/fiware-tech-summit-juanjo-gierro-fiware-overview-and-description-of-ges) |

If you are interested in more details about how to make your application a
context-aware application check out:

-   Using NGSI v2:
    -   [How to update and query context information](ngsi-v2/how-to-update-and-query-context-information.md)
    -   [How to subscribe to changes on context information](ngsi-v2/how-to-subscribe-to-changes-on-context-information.md)
    -   [How to perform geo-location queries](ngsi-v2/how-to-perform-geo-located-queries.md)

On the other hand, you can browse the full API description
[here](http://fiware.github.io/specifications/ngsiv2/stable/)

There is an early FIWARE NGSI HTTP binding, named NGSI v1 but it has been
largely overpassed by the current NGSIv2 version and it has been deprecated.

If you want to start experimenting and doing hands-on work, have a look at:

-   [Orion Context Broker GEri](http://github.com/fiware-ges/core.orion)
