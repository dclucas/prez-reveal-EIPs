# Enterprise Integration Patterns
 <!-- .slide: data-background="https://i.creativecommons.org/l/by/4.0/88x31.png" data-background-size="88px" data-background-repeat="none" data-background-position="2% 98%" -->



## base premises

v

I. system integration is a recurring problem;

v

II. tech varies, but the problems are similar in nature;


## unconfortable questions

v

a. why do we always reinvent the wheel?

v

b. why don't we have a standard lexicon for integration?


## unconfortable(r) answers

v

a. for no good reason whatsoever;

v

b. we do, and it's called Enterprise Integration Patterns;


## now for some definition...

v

An EIP represents a recurring element in integration

v

these elements may be endpoints, processors and channels


## hey, I love analogies! got some for me?

v

*EIPs are like Design Patterns for integration*

v

**true** because:

v

they provide a standard, platform-agnostic language

v

they can be described in terms of problems and how to solve them

v

they have become textbook material

v

**false** because:

v

they are much more platform agnostic

v

they are descriptive, not prescriptive

v

*EIPs are basically what ESBs do*

v

**true** because

v

this is really at the core of any ESB

v

ESBs and componentization have helped popularize EIPs

v

**false** because

v

not all ESBs implement all patterns

v

not all ESBs speack EIPese

v

ESB may and usually do a whole lot of additional things


## enough talk! show me the code!

v

(finally)

v

but...

v

we may not be talking about code, it's a lexicon...


## ok, then, so show me the ~~code~~ diagrams!

v

first, the basics

v

### Message
<!-- .slide: data-background="img/Message.png" data-background-size="400px" data-background-repeat="none" data-background-position="85% 50%" -->

v

### Endpoint
<!-- .slide: data-background="img/Endpoint.png" data-background-size="400px" data-background-repeat="none" data-background-position="85% 50%" -->

v

### Channel
<!-- .slide: data-background="img/Channel.png" data-background-size="400px" data-background-repeat="none" data-background-position="85% 50%" -->

v

### Publish/Subscribe Channel
<!-- .slide: data-background="img/Publish.png" data-background-size="400px" data-background-repeat="none" data-background-position="85% 50%" -->

v

## Example \#01:
1. read incoming files from an FTP
2. pass through a queue
3. pass it to a file share
<!-- .slide: data-background="img/SampleRoute01.png" data-background-size="600px" data-background-repeat="none" data-background-position="50% 90%" -->

v

## Example \#02:
1. read incoming files from a REST service
2. pass through a queue
3. pass it to staging table within a DB
<!-- .slide: data-background="img/SampleRoute01.png" data-background-size="600px" data-background-repeat="none" data-background-position="50% 90%" -->

v

*wait! please go back to the first example*

v

## Example \#01:
1. read incoming files from an FTP
2. pass through a queue
3. pass it to a file share
<!-- .slide: data-background="img/SampleRoute01.png" data-background-size="600px" data-background-repeat="none" data-background-position="50% 90%" -->

v

*now the second...*

v

## Example \#02:
1. read incoming files from a REST service
2. pass through a queue
3. pass it to staging table within a DB
<!-- .slide: data-background="img/SampleRoute01.png" data-background-size="600px" data-background-repeat="none" data-background-position="50% 90%" -->

v

a-ha! the diagrams are the same! copy-and-paste mistake!

v

not this time, little grasshopper

v

the diagrams are the same because the scenarios require the same **patterns**



## popular message processors

v

### Splitter
<!-- .slide: data-background="img/Splitter.png" data-background-size="400px" data-background-repeat="none" data-background-position="85% 50%" -->

v

### Content-based router
<!-- .slide: data-background="img/Router.png" data-background-size="400px" data-background-repeat="none" data-background-position="85% 50%" -->

v

### Aggregator
<!-- .slide: data-background="img/Aggregator.png" data-background-size="400px" data-background-repeat="none" data-background-position="85% 50%" -->

v

### Enricher
<!-- .slide: data-background="img/Enricher.png" data-background-size="400px" data-background-repeat="none" data-background-position="85% 50%" -->


## popular message patterns

v

### Event message
<!-- .slide: data-background="img/Event.png" data-background-size="400px" data-background-repeat="none" data-background-position="85% 50%" -->

v

### Command message
<!-- .slide: data-background="img/Command.png" data-background-size="400px" data-background-repeat="none" data-background-position="85% 50%" -->


# now let's do some whiteboarding...
(demo)


# tks


# References
[The book](http://amzn.com/0321200683)

[Reference web site](http://www.eaipatterns.com)

[Presentation engine](https://github.com/hakimel/reveal.js)

[license]: https://i.creativecommons.org/l/by/4.0/88x31.png