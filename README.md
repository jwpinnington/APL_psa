
# Intro

## The Map is Not the Territory

https://en.wikipedia.org/wiki/Map%E2%80%93territory_relation

# Context:

Our client runs a high volume B2B trading operation with large suppliers and business customers. We have provided a trading platform and other solutions for our client since 2016 (having provided solutions for other clients since 2007). 



# Scenario:

We have been asked to build a messaging application for use by our client to support operational dialogue with their suppliers and customers.

You have been asked to scope out the project and to consider different solution options. You have direct access to both the business client and technical teams.

## 1. What would your initial steps be?

\
 ![Screenshot1](./media/coiled_spring.png)

Uncoiling a spring.

### More context - First "know thyself"

Capabilities of the provider. 
It may seem obvious, but it is worth stating for the record that unlike a pure consulting role as solution architect where a solution may utilise methods and services from a potential array of technologies and providers, there is an [implicit bias toward those of the provider](#impact). Nothing untoward about this, one must pay the rent.

As such the solution architect must understand the territory from which they come and which they represent. First order of business for the solution architect is to map out the territory of the provider, perform the process of discovery on the business one is part of before going out to the client.

### Align solution within business and IT strategy of the client


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

#### <a name="inputs_1">
Background documentation: Model the existing actors that suport the objective; people, processes and technologies. From this we can begin to determine the [stakeholders](#inputs_3), actors ( process and technologies ). The goals of the objective. SMART: Specific, Measurable, Action-oriented, Realistic and Timely.

*'Adzic, Gojko. Impact Mapping: Making a big impact with software products and projects . Provoking Thoughts.'* 
    
#### <a name="inputs_2">
Solution vision document: this is a fleshing out of the given strategy.

#### <a name="inputs_3"> 
Stakeholder engagement

#### <a name="inputs_4">
Business requirements catalogue:
User - Actor stories

#### <a name="inputs_5">
Taxonomy

#### <a name="inputs_6">
Risk register

### Product Design

### Gap analysis

## 2. What would you expect the key success criteria to be?

The key success criteria of the solution would be the number of business requirements met.
The more business requirements met the higher the quality of the solution.

Of course the project as a process separate from the solution will have other basic success criteria beyond the scope ( business requirements ); is it on time and on budget.
The project could fail on time, on budget, or both, and the solution be a resounding success.

It is somewhat fuzzy. 

On a product view from the developement team success criteria may be stripped down to hard metrics, e.g.

     The API handler can accept ten times the requests per second than the previous version. This is a success, and clearly adds to the capabilities of the product, but may be incidental to the solution and the project.


~~*triple constraint fast/cheap/good of the project, separate from fast/cheap/good of the objectives driving the solution. Choose two.*~~


## 3. What constraints and barriers might you face?

Contraints may exist on both the client and provider side of the solution project.

* Time
* Budget
* Resources - human and material

Contraints to the solution.
* Discovery stage - Input
    * Barriers to communication
        * Nomenclature
        * [Access to stakeholders](#inputs_3) - 
        are full range of stakeholders in the room, have the end users, those at the coal face who would be using the product, been invited? *If you are not in the room, you are not in the deal.* ~~Is the real client business sponsor in the room, or is it a proxy? Good to have an idea of which.~~
        * ~~Scope - Mission creep - an inverse constraint~~

    * Business policies - these should be rolled into the business requirements / user - actor stories, but may not be explict, and could even be counter to a business requirement for the solution, e.g.
            
            Business policies: 'For staff work/life balance we have a rule of no emails after 6pm'. How does this apply to the messaging app, and how does this effect the usage and benefit of the app for the clients B2B partners?
    * Governance - Regulatory requirements
        * Data privacy, data residency
        * Other regulations pertaining to the market in which the B2B partners operate and may effect the content of the messaging
        * Best practice - standards on the product side
            * Accessibility - WCAG - ARIA
            * Internationalization - this is more of a business requirement if international clients.

* Technical contraints to the product
    * Capabilites
        * Does the provider have the technical capability to build product elements of the solution?
        * Do the end users of the client and it's B2B partners have the abilities to self-manage the product? The product should of course be simple to use. In the case of a human to human messaging app is there a requirement to manage enrolement and permissions governed by business rules? If so can the product be designed for self-service by business 'super users', and the solution be delivered with a 'train the trainers' approach for operational support? 
    * [Technology](#Technology)



## 4. At a high level, what architectural options might be relevant in this scenario?

\
Putting the scenario to one side for the moment; in a pure consulting role a solution architect may through discovery conclude that an option to achieve the client's business objective is not to build a messaging application, but to realign the client's particular procedures, personel roles and responsibilites to achieve the objective.

Options pertaining to the building of the messaging application:
* #### <a name="options2">Utilise capabilities of existing application portfolio
    * Upgrade / extend / configure existing application ( used by client ) with new functionality.
    * Create new application utilising modular components of provider's application portfolio.
* Create entirely new application ( which can be added to the application portfolio).
    * N-tier - this is on the territory
    * Micro-services - this is on the map


## 5. <a name="impact"> How might our client’s B2B environment and reliance on our existing systems impact on your recommendations?

There is a commerical logic to seek to align the solution within the business and IT strategy of the both the client and the provider. As such the implicit impact on the design would be to build upon the [reliance on existing systems](#options2) of the provider. 

The providers SaaS model lowers the technolgy risk of the solution for the client. It also ought lower the risk of the solution to the provider as the responsibility of the [non-functional requirements](#technologyNFR) lies solely with the provider and it's suppliers. Site reliabiltiy engineering has simple lines of control.

..The client's B2B environment 


### 6. Technology

Host environment - client device (OS, browsers\[webOS]\), and platform/server ability to run solution codes base

### <a name="technologyNFR">Non-Functional Requirements
* Security
* Audit
* Capcity
* Performance
* Availability
* Recoverability
* Robustness
* Integrity
* Maintainability


## 7. What project phases would you propose?

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
* [Requirements](#inputs_4) / User - Actor Stories
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
 ![Screenshot2](./media/project_phases.png)

## What technologies would you consider and how would you narrow down to final recommendations? What factors would you consider and who would you involve in this? 

Host environment - client device (OS, browsers\[webOS]\), and platform/server ability to run solution codes base
Who - primarily APL staff, client tech' staff (IT managers, Ops staff)
