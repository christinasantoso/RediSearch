Hey everybody, I’m Kyle and Meir will be joining us later to talk about CRDT and some benchmarks stuff, but I want to give you a little overview of RediSearch. So who here has heard of RediSearch before? Raise your hand. Anybody coming to my training on Monday? Well …(0:22) review for you. We’ll be seeing a couple of new things here.

[SLIDE] (0:36) 
```
RediSearch can be used for two [primary] things:
Full-text search | Secondary index
```

TRANSCRIPT

Okay, so let’s take a look at this, so RediSearch can be used for two primary things, right? The first thing it can be used for, is a full-text search and I think that’s what comes to mind when people think of search, right? They think of “Okay I’m gonna search for something in a body of human language, in the body of text” and it can be used for something else though, you know as we developed it for research. We figured out that people were using it for something else, they kind of using it for secondary indexing. So they had data stored somewhere else and they were using it to provide richer interfaces for their existing data that may be stored somewhere else in a way that wasn’t indexable.
So there are two [Inaudible 1.12] primary things we see people using it for, but there are some more use cases built into it. 


[SLIDE] (1:28) 
```
![slide1](RediSearch/Diagram.svg)
```

TRANSCRIPT

One of the things I want to show-- You can see my little laser pointer, right? It can be used for search and aggregation, right? And in the middle of this, I have in this Venn diagram querying. The reason I put it like this, is because they share the kind of same query language and share the same data as well. So there’s another functionality of RediSearch which I’ll go over briefly today which is autocomplete. Autocomplete isn’t-- I think really cool and not very used as much as some of these features but autocomplete does kind of type-ahead. So if you’re typing in a text box and you want to see what would come next, it can suggest it. It is important to know that these circles are not connected here. That is very relevant. The difference here is that they’re not connected because it uses an entirely separate set of data then the rest of this. So searching aggregation-- you can search an aggregator or the same thing, but autocomplete is entirely separate. So when you’re doing this you can use autocomplete with some other-- you know, search solution or some database solution or you know just searching through something that you have there. So to keep that in mind, when I talk about this, that he put something in search, it’s not necessarily gonna be an autocomplete but you can put it there if you want.
