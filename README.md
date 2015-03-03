# twitter-force-directed-graph

This is for the moment a fork of [d3-force-directed-graph](http://wtfleming.github.io//2015/02/19/d3-force-directed-graph/).

Currently it takes a JSON of nodes and edges and shows a visual representation of them.

It can be used to describe a Twitter account as a definition of the connections related to it.

I would like it to be more useful.

This is how I would like to augment it:

## TODO

### VERSION 1

- [ ] There should be a function that given a Twitter username fetches their followers and followings.
- [ ] The data returned should be formatted into the JSON structure described in `resources/public/test5.json`.
- [ ] There should be an input box that will accept this username and make an API request to fetch the json.
- [ ] After fetching the JSON it should use this to redraw the Graph.

### VERSION 2

- [ ] It should fetch data relating to the location of a Twitter account.
- [ ] It should colour a node depending on whether it has the same location as the main account.
- [ ] It should draw edges differently depending on their directionality.
- [ ] It should be able to output a list of usernames belonging to the location of the Twitter account.

### VERSION 3

- [ ] The size of nodes should depend on their follower count.
- [ ] It should allow multiple Twitter usernames to be passed in. This will create layered graphs.

### VERSION 4

- [ ] It should fetch the domain of an account. Either through some Twitter API, or through careful parsing of the Twitter accounts summary.

## Installation

```
lein cljsbuild auto
lein ring server-headless
```

## License

Copyright © 2015 William Fleming, Seb Insua

Distributed under the Eclipse Public License either version 1.0 or (at
your option) any later version.
