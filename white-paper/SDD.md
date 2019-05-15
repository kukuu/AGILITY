# The Software Design Specification aka SDD

Software architecture refers to the high level structures of a software system and the discipline of creating such structures and systems. Each structure comprises software elements, relations among them, and properties of both elements and relations.

Here, is an example structure of a  design document. This is a template and  should be adjusted as-needed. 


## Statement of Goals

Include a short paragraph describing the project and its intended audience.

## Functional Description

What does the application do? What application states (high-level descriptions of core user scenarios) will the user encounter?

For example, your functional description might look like:

```
First Run

Creating a New _____ (game, search, etc.)

Operations

Background and Foreground Behavior

```

## User Interface

Include wireframes for each page, with detailed descriptions of:

```
Each control, including states (enabled/disabled/highlighted) and operations.

Supported orientations and transitions between them.

Functionality represented.

Error handling.

Dimensions and constraints.

```


## Milestones

As described above, deadlines for completion and expected deliverables.

For example, the milestones section in your design document template might look like:

Facade Application showing screen and with temporary transitions and example images/text
Communication Protocol: application connects to network/server
Functional Milestone 1: …
Alpha Application (with full functionality)
Stability
Release



### Explaining the basics

```

FUNCTIONAL DESIGN DOCUMENT

A functional design document describes a software product's capabilities, appearance, 
and functions it needs to ultimately perform. Design documents are also referred to as
functional specifications or functional specifications documents (FSDs), or functional
requirements specifications.


HIGH-LEVEL DESIGN DOCUMENT?

A high-level design document (HLDD) describes the architecture used in the development 
of a particular software product. It usually includes a diagram that depicts the envisioned
structure of the software system. Since this is a high-level document, non-technical language
is often used.


SOFTWARE DESIGN DOCUMENT

Composition: data, architecture, interface, procedural

The software design document (SDD) typically describes a software product's "data" design, 
"architecture" design, "interface" design, and "procedural" design. The content and organization
of an SDD is specified by the IEEE 1016 standard.


DIFFERENCE BETWEEEN ARCHITECTURE & DESIGN

Typically, the design follows the architecture phase in a (new) system development process.
And while the architecture is rather "logical", the design is "physical", going down into the
detail of the implementation technology.

Functional requirement will describe a particular behaviour of function of the system when certain
conditions are met, for example: “Send email when a new customer signs up” or “Open a new account”.

```
