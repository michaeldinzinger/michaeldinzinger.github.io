User agent bias
===============

Previous studies on robots.txt files discuss a potential bias towards specific user agents. The hypothesis is that there exists a web-wide trend on the aversion of site owners and hence some crawlers are generally allowed to access smaller parts of websites than others. Analysis shows that such a bias definitely exists as the corresponding key figures vary significantly among user agents. The analysis comprises 14 product tokens (AdsBot-Google, AhrefsBot, Baiduspider, Bingbot, CCBot, ChatGPT-User, Googlebot, Google-Extended, GPTBot, ia_archiver, Mediapartners-Google, MJ12bot, PetalBot, Yandex) as well as a random reference user agent. As key figures, we have selected the average number of `allow` and `disallow` instructions per user agent. This goes along with a [study](https://doi.org/10.1145/1367497.1367711) from 2008, which evaluates the user agent bias by counting `disallow` instructions. Note that this is a rather course heuristic as it remains unclear how big is the part of the website, which is covered by the URL path in the `disallow` statement. Due to its ambiguity, we have thought about another key figure in order to analyze the popularity or antipathy among user agents, namely the total number of the *disallow all* instructions per user agent.
```
Example:
User-agent: GPTBot
Disallow: /
```
We assume a *disallow all* statement in case the robots.txt instructions prohibit the access of a URL pointing to a random address in the root directory of the website with only one `disallow` instruction stated in the robots.txt file. The following table