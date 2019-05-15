# The Software Design Specification aka SDD

Here, I’ll layout the example structure of a proper design document. Of course, this template should be adjusted as-needed. 


## Statement of Goals

Include a short paragraph describing the project and its intended audience.

## Functional Description

What does the application do? What application states (high-level descriptions of core user scenarios) will the user encounter?

For example, your functional description might look like:

First Run
Creating a New _____ (game, search, etc.)
Operations
Background and Foreground Behavior


## User Interface

Include wireframes for each page, with detailed descriptions of:

Each control, including states (enabled/disabled/highlighted) and operations.
Supported orientations and transitions between them.
Functionality represented.
Error handling.
Dimensions and constraints.
Here are the wireframes related to my latest iOS app, NotifEye:

These are the types of wireframes you might want to include in your software application design document.

If you’re interested, I made these mockups using Balsamiq’s wireframing tool.

For example, your UI description might look like:

Navigation Bar
...................
Left navigation control: return to home page
Title bar: current screen or operation name
New button: create a new Thing

Table View
.....................
Section 0: Section title
Section 0 rows:
Row control 0 (e.g., image)
Text Line 0
Text Line 2


## Milestones

As described above, deadlines for completion and expected deliverables.

For example, the milestones section in your design document template might look like:

Facade Application showing screen and with temporary transitions and example images/text
Communication Protocol: application connects to network/server
Functional Milestone 1: …
Alpha Application (with full functionality)
Stability
Release



Explaining the basics

```

FUNCTIONAL DESIGN DOCUMENT

A functional design document describes a software product's capabilities, appearance, and functions it needs to ultimately perform. Design documents are also referred to as functional specifications or functional specifications documents (FSDs), or functional requirements specifications.


A HIGH-LEVEL DESIGN DOCUMENT?

A high-level design document (HLDD) describes the architecture used in the development of a particular software product. It usually includes a diagram that depicts the envisioned structure of the software system. Since this is a high-level document, non-technical language is often used.


WHAT IS IN A SOFTWARE DESIGN DOCUMENT?

composition: data, architecture, interface, procedural

The software design document (SDD) typically describes a software product's "data" design, "architecture" design, "interface" design, and "procedural" design. The content and organization of an SDD is specified by the IEEE 1016 standard.



11. Functional and NFR (Non functional requirements)
NFRs are the requirements defined to cover the operational aspects of a product or an app while Functional requirement (FR) focus on the behavioral aspects.

NFR -  efficiency, portability, security, reliability, usability

For each of them a metric should be associated, and an acceptability level. In order to verify them, one should check if the contraints are satisfied & if the level of satisfation of the properties is greater than the acceptability level (with respect to the given metrics).

Software architecture refers to the high level structures of a software system and the discipline of creating such structures and systems. Each structure comprises software elements, relations among them, and properties of both elements and relations.


DIFFERENCE BETWEEEN ARCHITECTURE & DESIGN between Architecture & Design



Typically, the design follows the architecture phase in a (new) system development process. And while the architecture is rather "logical", the design is "physical", going down into the detail of the implementation technology.

Functional requirement will describe a particular behaviour of function of the system when certain conditions are met, for example: “Send email when a new customer signs up” or “Open a new account”.
