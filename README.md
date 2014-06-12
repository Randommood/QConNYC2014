# Computational Patterns of the Cloud
[QCon NYC 2014](https://qconnewyork.com/presentation/computational-patterns-cloud) - The Evolving Cloud Track - 4:15pm - 5:05pm ||
[Slides here for this presentation are up](https://speakerdeck.com/randommood/computational-patterns-of-the-cloud-qccon-nyc-2014)


The Cloud has undoubtedly changed the way we think about computing, IT operations, innovation, and entrepreneurship. But what are the computational patterns that have emerged from the pervasiveness of public clouds? What can we leverage to improve our organizations? And what are the challenges that we face going forward?

In this talk, I will introduce you to cloud computing’s paradigms and discuss their applications with practical examples from Engine Yard’s customers, peers, and partners. We will also cover antipatterns and myths. If you are curious about Cloud computing or want to improve your cloud strategy this talk is for you.

Images used in this talk are listed in the [credits](credits.md). (mostly) Everything I read to prepare this talk is conveniently listed for you in the [references](references.md) in case you want more.

# Tentative Agenda
*Content Goal: 50 minutes*

#### Reclaimable Resources
* Explanation
  * Pre-cloud architectures
  * Cattle vs Pets
  * The Myth of Elasticity
* Our experience with this pattern (our journey, customer stories)
  * Our story
  * Everything breaks at some point
  * Everything is a recipe/template
* Observed Challenges
  * Unpredictability of costs is an issue for customers
  * Importance of monitoring & benchmarking
  * Still need to understand resource families to fit use case

#### Harvesting Services
* Explanation
  * Local resources vs Services
  * Changes in app design for a clouded world
  * Consume services via APIs (SOA)
* Our Experience
  * The monorail that grew
  * Our new services
  * API mistakes
  * Consumers of IaaS APIs
* Observed Challenges
  * Monitoring, management, & analysis
  * What does 'healthy' mean?
  * Operational experience becomes siloed
  * Service dependency and failure planning
  * Importance of API design, maintenance & deprecation
  * The premature optimization dance

#### Distributed Systems as the new norm
* Explanation
  * Clustering
  * Consistency, Availability, Partition tolerance
  * Failures & degradation
* Our Experience
  * Coordination & availability of services (addons, stonith, serf)
  * Service tracing & impacts (find the request_id)
  * Failures become more interesting (recent story)
* Observed Challenges
  * Clustered everything requires operational proficiency
  * Making sense of metrics & collection display
  * What does it mean to be up?
  * Theoretical awareness matters
  * Distributed tracing becomes necessary (zipkin, dapper)

#### Continuous Everything
* Explanation
  * The way we work has changed
    * Continuous integration
    * Continuous delivery
  * Importance of tests
* Our Experience
  * Our continous integration
  * Evolution of our testing framework
* Observed Challenges
  * Unification of testing? Rectification of choices in framework
    * Rails: test-unit vs RSpec
    * Chef: test kitchen, chefspec, Serverspec, librarian, minitest-chef, sugar, bats, etc
* All planning tools suck
