## Vrooboo! Wabbo!!

Here is a summation of all relevant knowledge you should have learned before using the ruleset.

[uMatrix](https://github.com/gorhill/uMatrix) is a great browser extension, `point and click matrix to filter net requests according to source, destination and type`.

---

## Shagdovala - FAQs

1. What are principles on enabling third-party elements?

    The first prioirty  is to be sure most site function for normal browsing is working as how it is expected. The more elements is blocked despite that, the better.

2. It this enough (any other privacy tools recommened)?

    It is definitely not enough, some third-party elements contain both normal site facilities and also tracking scripts. Here are some others helpful:
    - [CanvasBlocker](https://github.com/kkapsner/CanvasBlocker)
    - [Cookie-AutoDelete](https://github.com/Cookie-AutoDelete/Cookie-AutoDelete)
    - [Decentraleyes](https://decentraleyes.org/)
    - [HTTPS Everywhere](https://www.eff.org/https-everywhere)
    - [Neat URL](http://hugsmile.eu/)
    - [uBlock Origin](https://github.com/gorhill/uBlock)

    Plus, if you re using [Mozilla Firefox](https://www.mozilla.org/firefox/all/), despite that battery API is removed to avoid being tracked, it is also suggested to navigation to:

    - `about:preferences#privacy`
        - at `History` section, select `Never` at `Accept third-party cookies`; check `Clear history when Firefox closes` option whose settings are suggested as at least `Cache`, `Site Preferences` and `Offline Website Data`.
        - at `Tracking Protection` section, select both `Always`
        - at `Permissions` section, check `Prevent accessibility services from accessing your browser`.
        - at `Security` section, **uncheck** `Block dangerous and deceptive content`: this uses Google Safe Browsing API and tracks your everywhere. Use pro anti-virus programs instead if necessary.
    - `about:preferences#search`
        - at `Default Search Engine` section, **uncheck** `Show search suggestions in address bar results`: the search engine provide will collect info if this is checked. If you rely on the suggestions, use engines that don't record things instead, e.g. DuckDuckGo.

3. How can I donate?

    [The owner](https://github.com/Rictusempra) has no any will to accept. Check how [other members](https://github.com/orgs/uMatrix-Rules/people) say.

4. What are these strange awkward words on this page?

    They are quotes of a character, `Gnar`, in an MMORPG called `League of Legends`. You may find all quotes [here](http://leagueoflegends.wikia.com/wiki/Gnar/Quotes).

## Gnar gada! - USAGE

1. First, choose a rule level you would prefer, [domain](https://github.com/uMatrix-Rules/uMatrix-Rules-Domain) or [site](https://github.com/uMatrix-Rules/uMatrix-Rules-Site).  It is recommended to choose the latter. Save the `rules.txt` into any local directory, or directly open it in your browser & copy all contents
2. open your uMatrix dashboard
3. navigate to `My rules` tab
4. import the rules:
   - click `Import from file...` and pick the file you just downloaded or;
   - click `Edit` and paste them from clipboard
5. edit as your like or click `Save`, and then `Commit`

## Shubbanuffa - BEFORE USING

- I can only ensure most site functions are workable. Use at your own risk.
- If you are expecting my investigation on any specific site, pls open a new issue at [corresponding place](https://github.com/uMatrix-Rules):
    - give a specific URL
    - point out your uMatrix version & broswer version
    - attach your own rules and, if differ from default, your preferences
    - If you are submitting issue on any site that requires account (cookies), a valid account mailed to the [org email address](lolipopplus@protonmail.com) may be necessary. By doing that you are trusting [org owner](https://github.com/Rictusempra) enough.
- Here are service inavailablity things that won't be fixed:
    -  from contents blocked by any built-in subscriptions
    -  caused by certain preferences outside of rule sets or of uMatrix itself
    -  if a site:
        -  is using cert from any untrusted CA
        -  containing **mostly only** pornographic content
        -  reported as a deceptive site
        -  is a private blog site that is not hosted on public serivce
    -  relevant with any plugin, such as Adobe Flash
    -  other issues you should have learnt from uMatrix [README](https://github.com/gorhill/uMatrix/blob/master/README.md) or [wiki](https://github.com/gorhill/uMatrix/wiki)

---

## Shugi shugi shugi - Some Temp. Rules

These rules should be used as temporary rules cleared as your browser closes rather than kept in uMatrix as permanent rules.
Such a behavior is suggested as these rules reserve usability on several pages while allowing tracking in very most parts on those sites.

Hint: you don't have to copy & paste them. Simply click uMatrix toolbar button and click on the corresponding square.

#### Baidu

    baidu.com fex.bdstatic.com script allow

#### Bilibili

    bilibili.com activity.hdslb.com script allow

#### Youku

The rules given here should work fine. If not, disable the scope & hard refresh (without cache), and enable again as soon as any video starts. Still no idea why.

---

## Ovagarava - T.O.C.

- [Blacklist Mode](/Blacklist-Mode.md)
- [Contributing Guidelines](/Contributing.md)
- [Cookies Control](/Cookies-Control.md)
- [Differeces Between uMatrix and uBlock Origin Advanced Mode](Differences.md)
- [uMatrix Friendly Sites](/uMatrix-Friendly-Sites.md)
- Third Party Iframe
    - [Google Service](/Google-Services.md)
    - [Video Iframe Examples](/Video-Iframe-Examples.md)
    - [Others](/Others.md)

### Reeshoova! - LICENSE
<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a>
Except where otherwise noted, all content in this org is licensed under the <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">CC BY-NC-SA 4.0 International License</a>
