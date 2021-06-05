# The OfficiumDivinum Project

There are many excellent projects to make computers speak liturgically. The
[gregorio](https://gregorio-project.github.io/) project makes producing
beautiful chant scores easy (and TeX and LaTeX make producing beautiful
documents easy); [divinumoficium](https://divinumofficium.com) makes the divine
office (from the pre-tridentine monastic books through to the final reforms
before it was replaced with the *Liturgia Horarum*) and the Mass in the ancient
Roman rite available in many languages to anyone with an internet connection;
[gregobase](http://gregobase.selapa.net) from the gregorio project contains
almost the entirety of *all* the major chantbooks; and Benjamin Bloomfield's [psalm
tone tool](https://bbloomf.github.io/jgabc/psalmtone.html) (or
[pslm](https://github.com/igneus/pslm)) can point psalms for chanting.

The only problem with these and many other excellent projects is that they are
generally written for programmers, by programmers, or as standalone applications
for a specific purpose. Divinumofficium has errors in it, but correcting them
requires understanding its (rather elegant) adhoc database structure, and not
being intimidated by the words like 'pull request'.[^1] Gregobase has
everything, but it is not possible to search or retrieve scores
programmatically.[^2]  Bloomfield's work is excellent, but if you're making a
booklet you still have to put everything together by hand.

OfficiumDivinum aims to be the missing glue to hold everything together.

* Lots of people are very knowledgeable about Liturgy, but can't write code.
* Lots of people are very good at writing modern web apps, but not so at home
  with the interactions of TeX, fonts and a music typography layer built on top
  of TeX (not to mention whole websites written in perl, like divinumofficium).
* Lots of other people are very good at writing web APIs and standalone code,
  but not so good at writing frontend stuff like web apps.
  
On the other hand

* Everyone can use a point-and-click WYSIWYG app

Thus we offer:

* A complete re-write of the logic from divinumofficium as a fully documented
  [OpenAPI compliant backend api](https://2e0byo.co.uk/docs) (**WIP**)
* An [example web app](https://2e0byo.co.uk) for the divine office written in
  Vue.js, which will ultimately have WYSIWYG editing. (**TODO**)
* A set of
  [parsers](https://github.com/OfficiumDivinum/OfficiumDivinum/tree/master/backend/app/app/parsers)
  for divinumofficium's source files, which drop out nice python objects you can
  use directly in your own code.
* Documentation for the divinumofficium database structure, which is hopefully
  easier to read than the perl. (**TODO**)
* A booklet generator integrated with the office, to make singing any office
  together *easy*. (**WIP**)
* Tools for standardising gregorian scores, so that booklets display in a
  standardised fashion. (**TODO**)
* Testsuites and documentation for everything.

[^1]: The divinumofficium team are extremely quick to merge pull requests,
    however!

[^2]: We are working on a PR to fix this at the moment.
