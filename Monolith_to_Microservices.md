# Monolith to Microservices

`architecture` `book`

![Screen_Shot_2023-01-05_at_19-45-09.png](image/Screen_Shot_2023-01-05_at_19-45-09.png)

## Chapter 1. Just enough Microservices

### What are Microservices

- Independent deployability (loosely coupled)
- Modeled around business domain (not layered architecture)
- Own their own data
- Advantages
    - scale 
    - robustness (smaller blow radius)
    - varied technologies
    - flexibility
- Disadvantages
    - network overhead
    - distributed transactions are complex 

### Monoliths

- single process
- distributed (coupled services)
- third-party black box
- modular (Spotify)
- issues
    - implementation and deployment coupling
    - blurred team responsibility lines
- advantages
    - simplified monitoring, thoubleshooting, testing
    - easier code reuse

Information hiding (Parnas) goes beyond classes (services expose APIs and hide details)

## Chapter 2. Planning the migration

### Why choose M.?

- improve team autonomy (alternative - modular monolith)
- reduce time to market (not a problem if you releases are easily coordinated)
- scale cost-effectively for load (only if scaling monolith does not work well)
- improve robustness (microservices won't solve it by default, redundant replicas could be used with monolith as well)
- scale the number of developers

When M. are bad?

- unclear domain
- startups
- customer-managed software (desktops)

### Buy-in

- make sure one of the above reasons is sponsored (What) the only question is How
- Dr. John Kotter’s eight-step process
    - establish a sense of urgency (find a precedent)
    - create the guiding coalition
    - develop a vision and strategy 
    - communicate the Change Vision (not a single message)
    - empower employees for broad-based action (remove roadblocks, help find time)
    - generate short-term wins
    - consolidate gains and produce more change (analyze and course correct)
    - anchor new approach in the culture

- incremental migration !
- only services in production count

Where to start?

- DDD, Event Storming
- use domain model for prioritization (start from bounded concepts with the least number of incoming dependencies)
-  Team Topologies
- changing personal skills 

Do regular checkpoints.

Avoid Sunk Cost fallacy.
