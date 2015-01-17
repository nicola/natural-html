# natural-html
Writing HTML in Natural Language

## The idea
Not everyone can write code, but many can imagine how things should look like. This challenge aims at stimulating interest in researching new ways to write HTML using Natural Language.

## Example

The following is an example of what **ntml** should look like:

```
> Start a new page
OK
+ <html>
+ <head>
+   <title></title>
+ </head>
+ <body>
+ </body>
+ </html>

> Name the page, the amazing page
OK
-   <title></title>
+   <title>The amazing page</title>

> Add a div in body called #main
OK
+ <div id="main"></div>

> Put #main in center of the page
Ambiguity
1) Size not specified
2) Fixed or relative size?

+ #main { margin: 0 auto; width: 70%; }

> No, make #main fixed
OK
- #main { margin: 0 auto; width: 70%; }
+ #main { margin: 0 auto; width: 900px; }

```

## Dataset

I am thinking of writing a little dataset with some basic use cases

## Approaches

There are many ideas that I have in mind on how to tackle this:

- Image vision and reinforcement learning to see if things are like they are described (the machine tests all the properties out), however this might lead to very bad quality HTML
- First-order logic or lambda representations that map to HTML. In addition, in we can combine distributional models to understand the meaning of content words
