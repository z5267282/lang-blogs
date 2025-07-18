# Overview

Each JSON file will contain a list of HTMLElements.

```txt
[
    HTMLElements...
]
```

# Objects

Each HTMLElement will be mapped to the following object structure.

## Header

```txt
{
    "type" : "Header",
    "level" : <number>,
    "content" : <string of header value>
}
```

## Code

```
{
    "type" : "Code",
    "language" : <string of language suffix - can be empty>,
    "code" : [<string of code lines>]
}
```

## Ordered List

```
{
    "type" : "OrderedList",
    "items" : [<string of list items where index has been stripped>]
}
```

## Unordered List

```
{
    "type" : "UnorderedList",
    "items" : [<string of list items where leading "- " has been stripped>]
}
```

## Paragraph

```
{
    "type" : "Paragraph",
    "lines" : [<string of content where trailing "  " has been stripped>]
}
```
