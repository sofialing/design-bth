---
views:
    main:
        template: anax/v2/article/default
        data:
            class: blog

    byline: false
    block-about: false
    article-toc: false

    blog-list:
        region: main
        template: anax/v2/blog-list/default
        sort: 2
        data:
            dateFormat: j F Y
            meta:
                type: toc
                orderby: publishTime
                orderorder: desc

    blog-toc:
        region: sidebar-right
        template: anax/v2/blog-toc/default
        sort: 2
        data:
            title: Inlägg
            meta:
                type: copy
                view: blog-list

---
Dagens bild
===========================

Kortare blogginlägg om vad som händer på dbwebb.se, kurserna samt webbprogrammering och webbutveckling med HTML, CSS, JavaScript, PHP och SQL i allmänhet.
