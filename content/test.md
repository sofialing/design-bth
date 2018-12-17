---
views:
    breadcrumb:
        region: breadcrumb
        template: anax/v2/breadcrumb/empty
        data:
            meta:
                type: breadcrumb
    kursrepo:
        region: sidebar-left
        template: anax/v2/block/default
        data:
            meta:
                type: single
                route: block/om-kursrepo

    redovisa:
        region: sidebar-right
        template: anax/v2/block/default
        data:
            meta:
                type: single
                route: block/om-redovisa
    start-image:
        region: after-main
        template: anax/v2/block/default
        sort: 3
        data:
            meta:
                type: single
                route: block/start-image
    flash-text:
        region: flash
        template: anax/v2/block/default
        data:
            meta:
                type: single
                route: block/flash-text
---
Test med olika konstruktioner av Markdown
=========================

Det här är en h2-rubrik
---------------------


### Det här är en h3-rubrik

Det här är en text med en *betoning* av ett ord.
Det här är också en _betoning_.

* Katt
* Hund
* Häst

1. Katt
2. Hund
3. Häst

Det här är en [länk](http://google.com/).

![alt text](img/dator.jpg "Titel")
