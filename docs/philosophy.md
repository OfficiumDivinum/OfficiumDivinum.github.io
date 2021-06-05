# Philosophy

!!! note
    By *philosophy* we mean 'how we set about doing things', i.e. *policy*.
    
## Rationale

The Liturgy of the Catholic Church is eternal.[^1]  The form of that liturgy here
below changes but slowly (except when something pretty much brand new is
substituted for it).  The internet is very young, and everything on it is
already old.  Thus divinumofficium, which is an incredible resource, is written
in a declining language (perl), using a home-made database format, in a time
before 'paradigms' were really so important, turning out hand-formatted
unstructured html.  Anything we write will look this way in fifteen years time:
perhaps less, because Laszlo Kiss was an incredible programmer.

!!! summary
    The websites of an Eternal Church should be old and every young, capable of
    serving up from their databases treasures *nova et vetera*, whatever the
    internet may look like in the future.
    
## In Practice

`If it's not documented, it's not finished.`
 : Documentation should be readable by a tinkerer in the language in question,
   and thorough enough to enable complete reimplementation in the future.

`Build modular tools with well defined interfaces.`
 : The easier tinkering is, the easier it will be gradually to replace
   infrastructure.
   
`Test everything which can be tested.`
 : Tested code is less brittle code.  And people might get involved in less
   brittle code.
   
`Automate as much as possible.`
 : Anything which can be run on an automation server should, so contributors
   only have to supply new code, and everything else will drop into place.
   
`Plan for obselescence.`
 : Code should die gracefully; and new code should take its place.
   
`Document your design decisions, not just your implementation.`
 : Including these!  Explaining *why* a particular approach was taken is almost
   as important as explaining how it works.  Perhaps more so, as anyone can read
   the code to figure out how it works.


[^1]: For the form taken by the *sacrificium laudis* here below, bound up as it
    is with the Sacrifice of Calvary, is temporal, but as George Macdonad put
    it, on Calvary the Son 'did that, in the wild weather of his outlying
    provinces, which he had done at home in glory and gladness,' and thus
    liturgy itself points to something eternal.
