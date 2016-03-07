#SUBconscious

SUBcoscious (or SUB for short) is your new creative thinking partner, powered by artificial creativity and global subconscious of the world wide web.

--------

## Theory

* Creativity is combinatorial in nature: subconscious is constantly generating gazillions of random combinations, filters them and beams the more interesting ones back to the consciousness prompting it to explore and evaluate randomly established connections between various images and experiences. Conscious then acts as an editor, but not the originator.
* Computers are good at combinatorial tasks and dealing with a lot of data.
* The Internet (as a system of multiple humans and multiple computers connected together) is a giant collection of content with some connections between content items - and this collection is always bubbling and producing more
* If we could only tap into this "global subconscious" productively, augmenting our own collection of experiences and memories by those of all the other Web users - we could produce a lot of interesting creative stuff.
* Beyond the practical value of being able to come up with more and better ideas, there is a more interesting implication: Extending our subconsciousness by sharing it can be the first step into extending our consciousness by sharing it as well. Whether this later is a viable and good step - only God knows.
* SUB can be seen as a necessary first step to AGI. I.E. if consciousness is an emerging layer of complex filtering + framing + reduction function, then it has to work on top of the previous layer, containing living and pulsating information structure. SUB is a first attempt at creating this base layer on top of which consciousness may arise. When refering to AGI, I don't necessarily mean an independently electronic / mechanical strucutre, but possibly a hybrid consiting of many
  humans and many machines.

--------

## Key ideas and definitions

* User - human who is using our system to help him / her come up with more interesting thoughts
* SUB - an instance of our system that has persistent memory and interacts with the User to prompt him / her with images that can spark thoughts or ideas
* Brain - individual SUB's core that consists of:
    * Clock - stepping and sync, controlling the working of the brain in steps
    * Interpreter - simple input analyzer
    * Instructions - set of pre-defined instructions that trigger certain actions
    * Memory - weighted graph of Images and Associations (see below)
    * Impulse - element of randomness (based on random machine or pre-determined input) - used to navigate Memory and send to filter
    * Filter - dynamically adjusted logic for filtering the results of brain working and deciding whether to send back to the user or not
    * Formatter - formats the output and sends it back to the user
    * Output queue - queue of things ready for user output
* Attention - an internal set of pointers representing where SUB's focus currently is inside the Memory graph of the SUB.
* Memogination (memory + imagination + memory generation) - an act continuously performed by an indivudual SUB's brain that results in the stream of subconsciousness being outputted to the user. Memogination works as follows:
    * SUB's several points of attention continuously wander around SUB's Memory graph, their movement directed by random Impulse and the force / weight of Associations. As they travel - new associations are created and stored in the Memory.
    * At every step of the clock any one of the attention pointers (selected randomly?) makes a move. The new position of pointers represents a current thought.
    * This thought is filtered and evaluated for originality and potential interest and then (if it passes the filters) - is added to the output queue.
* Stream [of subconsciousness] - a session of interaction between a user (or group of users) and a SUB.
* Image - a single content item inside a Stream (it can be a textual, visual or audio).
* Thought - a particular combination of Images inside a stream
* Stream state - current state of the stream, represented by:
    * Weighted graph of Images and their interconnections at a given moment, specific to the current stream
    * Current thought - combination of images currently displayed to the user
    * History of user input, stream output and build-up of the graph
* Association - a weighted connection (relationship) between various images (specific to current Stream or generally persisted forever inside individual SUB's brain)
* Snapshot - a graphical representation of a Thought (a particular state of the Stream).

--------

## How it works (User Scenario)

1. You start a new Stream or continue an old one.
2. You talk to your SUB, using natural language in a chat interface. You highlight keywords that SUB should pay attention to by prepending `#` before them. e.g. `We need to come up with a way to solve #death`
3. Based on your input and its own associations, SUB continuously fills the Stream with Images (words, visuals and sounds). Some of those Images are based on searching the internet for your keywords or combinations of them, other Images are based on synonyms / antonyms and other derivatives or combinations of your keywords, still others are completely random. You are not presented by one Image at a time, but instead by a few at any given moment and as some fade away - new ones appear.
4. At any point if you find something interesting you can pause your stream by saying `SUB, pause`. You can then roll your Stream back in time and look back at particularly interesting items and combinations of items (thoughts).
5. At any point you can take a snapshot of the current thought.
6. When you are ready to terminate a thinking / dreaming session - simply say `SUB, enough`. You can save your entire stream or the snapshots you've taken (as images) - should you want to get back to them later. 
7. Even when you are not in a session, you may sometimes want to save something to your SUB, so that it is added to your SUB's memory and can spring back at your later. You can simply email any content to your SUB or clip anything from the web into your SUB using our browser plugin. This content will be added to your SUB's memory and will be brought back to you in your future sessions.
8. Sometimes you may want to search your SUB's memory to find a particular Thought or Image. Inside any stream simply type `SUB, search "something and something"` and you will see search results appearing in your stream.

--------

## How it works (inner logic)

* Upon the start of a new stream, a new stream node is created in the graph memory of the Sub with a unique ID. E.g. `Stream_fywoeriu23gfi`. Fixed number (e.g. 3) of attention pointers are all pointing at the stream node. 
* Clock is ticking at `TPS` (ticks per second)
* At each tick:
    * we evaluate user input made since the previous tick and make changes to the Mass and Velocity of attention pointers and Memory (if needed - new nodes are created and connected to others and to Tao). Occasionally based on user input a random pointer can be moved to a completely new node. Another way of thinking about it is to say that attention points are always jiggling around but we are giving them energy that can help them make a quantum leap elsewhere.
    * then run Memogination once
    * Memogination changes the position of one or more of the attention pointers (which one is decided randomly, but takes into account a the `mass` and previous `velocity` of each attention pointer i.e. it's reluctance to change it's state of motion). After we give energy to the attention pointer may or may not gather enough energy to make a Jump from this memory node (image) to some other node. A jump can take the attention pointer to:
        * a node inside the same stream
        * a node inside a different stream, but belonging to the same SUB
        * a node to a different stream, belonging to a different SUB
        * a newly created node that is taken from the outer world (by searching WWW)
    * Whether or not an attention pointer is going to jump and where to depends on the overall topology of the space, its mass & velocity (energy level) and some random element as well. Each node can have a weight to indicate how much energy it takes to get out of it: think of a sticky melody as a node with a very big mass. All in all this can be visualized similarly to the way gravitation field is visualized.
    * With every jump of attention pointers - a new connection between the fromNode to toNode is created (or an existing connection is strenghtened - like establishing connections between neurons).
    * Memogination spits out a new Thought i.e. an array of Images (content nodes) that pointers are currently pointing to. This thought goes to the Filter.
    * Filter evaluates the thought's originality and level of interest (based on whether this or similar through has been shown before and user reaction to it or similar thoughts in the past)
    * With every new generated thought - a new connection is established between all the nodes that are a part of the thought (i.e. "Fire together - wire together"). If a thought passes through a filter - the connection is stronger. If a thought is later highlighted / praised by the user, connection is made even stronger.
    * If Filter decides that a thought is interesting enough - it adds a thought to the top of the Output Queue
* User view changes at `FPS` (frames per second) + randomized to create a more natural feeling
* At each view change:
    * A new thought is taken from the top of the Output Queue
    * The Images that stay the same as in the last displayed Thought stay on the screen
    * Images that are gone (compared to the previous thought) - fade out
    * Images that are new (compared to the previous thought) - fade in

--------

## Business Model

SUBconscious is open source software that you can install and use on your machine.
However we offer a hosted version that is:

* Simpler - nothing to install or configure
* Smarter - used by more people and so learning much faster

### Pricing for hosted SUB

* Everybody's SUB - forever free - no registration, no persistent Streams, no individual learning, all streams are public.
* Your SUB - $250/year - unlimited persistent private streams, individual learning, invite up to 3 people into your sub.
* Group SUB (for teams of 5+) - $100/user/year - multi-user Streams, individual + team learning.
  
--------

## Tech Stack

* Platform: WEB
* Framework: [Meteor](http://meteor.com)
* Graph DB: [neo4j](http://neo4j.com/)
    * Hosted: [GrapheneiDB](http://www.graphenedb.com/)
    * Meteor package: [neo4j for Meteor](https://github.com/VeliovGroup/ostrio-neo4jdriver)

--------

## DONE

* write down basic concept and key ideas
* create the story and register domain
* learn the basics of graph theory and possible graph db implementations (Neo4J)
* install Neo4J
* setup the project structure (scaffold with Iron)

## TODO

* do a test for Neo4J & Meteor interaction
* create basic interface
* implement chat
* implement simplest SUB stub: it just adds keywords from the chat to the Memory and at then randomly shows combinations of those keywords
* implement some more intelligent node manipulation: for every user inputted keyword - add more nodes (synonyms / antonims, google image results for this word, google translate results for this word, related words [by doing google translate back and forth] etc.)
* implement smarter filtering (google search for word combinations and based on search results adding new nodes to the Memory)
