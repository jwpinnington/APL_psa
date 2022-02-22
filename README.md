
# Intro

## The Map is Not the Territory

https://en.wikipedia.org/wiki/Map%E2%80%93territory_relation

# Context:

Our client runs a high volume B2B trading operation with large suppliers and business customers. We have provided a trading platform and other solutions for our client since 2016 (having provided solutions for other clients since 2007). 



# Scenario:

We have been asked to build a messaging application for use by our client to support operational dialogue with their suppliers and customers.

You have been asked to scope out the project and to consider different solution options. You have direct access to both the business client and technical teams.

## What would your initial steps be?

### More context

Capabilities of the provider,




### Align solution within business and IT strategy of the client
\
VMOST

| Initial | word      | Business/IT |
|---------|-----------|-------------|
| V       | Vision    |  BBBBB      |
| M       | Mission   |  BBBBB      |
| O       | Objective |  BBBB/T     |
| S       | [Strategy](#inputs_2)  |  BBB/TT     |
| T       | [Tactics](#inputs_4)   |  B/TTTT     |

The Scenario exists at the level of a strategy, a messaging application, and an objective which is to support operational dialogue with suppliers and customers.

Is the objective extant, or is it a new objective? The context would lead to an assumption of the objective being extant. Much as we wish to talk about the journey into the future we should [map the territory](#inputs_1) where we are.

~~*“I wouldn’t start from here if I were you.”*~~

The [strategy](#inputs_2) is a change state to the objective, strategy is the vector to the objective's scalar. Here we begin to [map a territory](#inputs_2) that does not yet exist.

The [tactics](#inputs_4) are the means by which which areas of our map of the territory to be built are sketched out.

    
### Solution architecture inputs

#### inputs_1
Background documentation: Model the existing actors that suport the objective; people, processes and technologies. From this we can begin to determine the [stakeholders](#inputs_3)
    
#### inputs_2
Solution vision document: this is a fleshing out of the given strategy.

#### inputs_3
Stakeholder engagement

#### inputs_4
Business requirements catalogue:
User stories

#### inputs_5

Taxonomy

#### inputs_6 

Risk register


### Product Design

### Gap analysis

## What would you expect the key success criteria to be?

The key success criteria of the solution would be the number of business requirements met.
The more business requirements met the higher the quality of the solution.

Of course the project as a process separate from the solution will have other basic success criteria beyond the scope ( business requirements ); is it on time and on budget.
The project could fail on time, on budget, or both, and the solution be a resounding success.

It is somewhat fuzzy. 

On a product view from the developement team success criteria may be stripped down to hard metrics. The API handler can accept ten times the requests per second than the previous version, 
this is a success, and clearly adds to the capabilities of the product, but may be incidental to the solution and the project.


~~triple constraint fast/cheap/good of the project, separate from fast/cheap/good of the objectives driving the solution.~~


## What constraints and barriers might you face?

Provider 

Nomenclature

Time, access, barriers to communication, methods of communication. 

Client 

Funding / Resources

Capabilities


Government / Compliance / Standards

regulatory requirements, the bribery and corruption act, data privacy, data residency.

WCAG - ARIA


Business policies: *'no emails after 6pm'*
International clients, Internationalization



## At a high level, what architectural options might be relevant in this scenario?

\
Putting the scenario to one side for the moment; in a pure consulting role a solution architect may through discovery conclude that an option to achieve the client's business objective is not to build a messaging application, but to realign the client's particular procedures, personel roles and responsibilites to achieve the objective.

Options pertaining to the building of the messaging application:
* Utilise capabilities of existing application portfolio.
    * Upgrade / extend / configure existing application ( used by client ) with new functionality.
    * Create new application utilising modular components of provider's application portfolio.
* Create entirely new application ( which can be added to the application portfolio).
    * N-tier - this is on the territory
    * Micro-services - this is on the map


## How might our client’s B2B environment and reliance on our existing systems impact on your recommendations?

Host environment - client device (OS, browsers\[webOS]\), and platform/server ability to run solution codes base

Non-Functional Requirements

Security, Audit, Capcity, Performance, Availability, Recoverability, Robustness, Integrity, Maintainability, Usability, Documentation


## What project phases would you propose?

For the solution architecture stream of the project: 
* Initiation 
* Discovery
    * [Architecture Inputs](#solution-architecture-inputs)
    * [Stakeholder engagement](#inputs_3)
    * [Business requirements](#inputs_4)
* Solution Outline
* Analysis
* Logical Design
* Validation
* Roadmap
* Completion

For the product management stream of the project:
* Discovery
* [Requirements](#inputs_4) / User Stories
* Product / Feature backlog
* Sprint loop 
    * Sprint plan
    * Design and build
    * UAT
    * UAT bug fix / snagging
    * Release
    * Retrospective - leasons learned
    * GOTO - Sprint plan

\
The phases of the two streams align somewhat as per the image below:

\
 ![Screenshot1](./media/project_phases.png)

## What technologies would you consider and how would you narrow down to final recommendations? What factors would you consider and who would you involve in this? 

Host environment - client device (OS, browsers\[webOS]\), and platform/server ability to run solution codes base
Who - primarily APL staff, client tech' staff (IT managers, Ops staff)
