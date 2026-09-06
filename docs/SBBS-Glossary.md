# SBBS Glossary

## Smart Black Box System (SBBS)

### Definition

Smart Black Box System (SBBS) is an AI-Native software architecture
that organizes software systems as reusable capability units.

Unlike traditional software reuse based on reusable code,
SBBS focuses on reusable intelligence:

- Capability
- Knowledge
- Rules
- Contracts
- AI-readable descriptions

A SBBS system is assembled from independent Smart Boxes,
connected through Smart Wires, coordinated by Assemblies,
and presented through Components.


---

# Core Concepts


## 1. Capability

### Definition

Capability is an independent ability that a system provides,
regardless of its implementation technology.

Capability answers the question:

"What can the system do?"

Examples:

- storage
- search
- authentication
- assessment
- recommendation
- reasoning


### Principle

SBBS follows:

Capability First

Capability → Contract → Implementation


The capability must exist before choosing
any technical implementation.


---

# 2. Smart Box

## Definition

A Smart Box is a self-contained capability unit
that encapsulates business logic, knowledge,
rules and AI-readable descriptions.


A Smart Box is not simply a software module.

It contains:


- Identity
- Specification
- Interface Contract
- Implementation
- Knowledge
- Rules
- AI-readable Description


## Responsibility

A Smart Box owns:

- business capability
- domain logic
- data model
- validation rules
- operational behavior


## Boundary

A Smart Box does NOT know:

- where it is displayed
- where data is stored
- which infrastructure technology is used


## Example


SBBox-001-Prompt-Note-Manager

Capability:

Manage AI prompt notes.


Possible implementations:

LocalStorage
Supabase
Cloud Database


The Smart Box remains unchanged.


---

# 3. Smart Wire


## Definition

Smart Wire is the intelligent communication layer
connecting capabilities.

It separates:

WHAT the system needs

from

HOW technology provides it.


## Responsibility

Smart Wire handles:


- data transmission
- format transformation
- validation
- error handling
- security
- monitoring
- context transformation


## Architecture


Capability Layer

↓

Contract Layer

↓

Implementation Layer


Example:


storage capability


can use:


Wire-Adapter-LocalStorage

or

Wire-Adapter-Supabase


---

# 4. Wire Adapter


## Definition

Wire Adapter is a concrete implementation
of a capability connection.


Example:


Capability:

storage


Adapters:


Wire-Adapter-LocalStorage

Wire-Adapter-Firebase

Wire-Adapter-Supabase


## Principle

Changing Adapter must not modify Smart Box logic.


---

# 5. Assembly


## Definition

Assembly is the orchestration layer
that combines independent capabilities
into a complete application.


Assembly decides:

- Which Smart Boxes are used
- Which Components are connected
- Which Wire Adapter is selected


## Important Rule


Assembly does not create new capability.

Assembly only assembles existing capability.


---

# 6. Component


## Definition

Component is the human interaction layer.

It presents capability results
to users.


Examples:

- Web interface
- Mobile interface
- Dashboard
- Visualization


## Boundary


Component must not directly access:

- Database
- Infrastructure API
- Internal Box implementation


Component communicates through contracts.


---

# 7. Contract


## Definition

Contract is a formal agreement
between system capabilities.


It defines:

- Input
- Output
- Rules
- Constraints


Contract allows independent evolution
of components.


---

# 8. Knowledge


## Definition

Knowledge is domain information
that allows humans and AI systems
to understand a capability.


Examples:


Knowledge.md

Examples.md

Domain documentation


Knowledge transforms code
into understandable intelligence.


---

# 9. Rules


## Definition

Rules describe constraints
that control system behavior.


Examples:


- Validation rules
- Business rules
- Safety rules
- Decision rules


Rules allow AI Agents
to reason about capability usage.


---

# 10. AI-readable Architecture


## Definition

AI-readable architecture means
that system structure and capability descriptions
are understandable by AI Agents.


Every Smart Box should provide:

- Identity
- Specification
- Contract
- Knowledge
- Rules
- Examples


This enables AI discovery,
selection and assembly.


---

# 11. Registry


## Definition

Registry is a discovery mechanism
that stores information about available capabilities.


Future SBBS Registry may contain:


- Smart Box list
- Capability metadata
- Version information
- Compatibility information


Registry enables automatic discovery
by humans and AI Agents.


---

# 12. AI Agent


## Definition

An AI Agent is an autonomous intelligence
that can discover, reason about,
and interact with SBBS capabilities.


Future SBBS versions may allow Agents to:

- search capabilities
- select Smart Boxes
- compose Assemblies
- evaluate compatibility


---

# 13. Reusable Intelligence


## Definition

Reusable Intelligence is the core philosophy
of SBBS.


It means reusable units contain not only code,
but also:

- meaning
- knowledge
- rules
- interfaces
- operational context


SBBS moves software engineering from:

Reusable Code

to

Reusable Intelligence.


---

# 14. AI-Native Software Architecture


## Definition

AI-Native Software Architecture is an approach
where software systems are designed
for collaboration between humans and AI.


Software is not only executable by machines,
but understandable and discoverable by AI.


---

# Version

SBBS Glossary v0.1.0

Foundation vocabulary for Smart Black Box System.
