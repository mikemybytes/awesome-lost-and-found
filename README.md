# Awesome lost & found

A personal list of useful software engineering resources that may have been lost in my browser's history otherwise.

## Architecture

- [The Twelve-Factor App](https://12factor.net/)
- [A Hitchhiker’s Guide to Caching Patterns](https://hazelcast.com/blog/a-hitchhikers-guide-to-caching-patterns/)
- [Microservices Production Readiness Checklist](https://github.com/kgoralski/microservice-production-readiness-checklist)
- [Simple systems have less downtime](https://www.gkogan.co/blog/simple-systems/)
- [Event-Driven Architectures vs. Event-Based Compute in Serverless Applications](https://www.alexdebrie.com/posts/event-driven-vs-event-based/) - using 
serverless functions (like AWS Lambda) is not enough to call the architecture "event-driven" 

## Java

- [Maintaining a medium-sized Java library in 2022 and beyond](https://michael-simons.github.io/neo4j-migrations/maintaining-a-medium-sized-java-library-in-2022-and-beyond/)
- [Modern Best Practices for Testing in Java](https://phauer.com/2019/modern-best-practices-testing-java/)
- [Map.merge() - One method to rule them all](https://nurkiewicz.com/2019/03/mapmerge-one-method-to-rule-them-all.html)
- [What is the point of extending a sealed class with a non-sealed class?](https://stackoverflow.com/questions/63860110/what-is-the-point-of-extending-a-sealed-class-with-a-non-sealed-class/63887136#63887136)
- [How the JIT compiler boosts Java performance in OpenJDK](https://developers.redhat.com/articles/2021/06/23/how-jit-compiler-boosts-java-performance-openjdk)
- [Automatic-Module-Name: Calling all Java Library Maintainers](http://branchandbound.net/blog/java/2017/12/automatic-module-name/)
- [Testing in a modular world](https://info.michael-simons.eu/2021/10/19/testing-in-a-modular-world/) - an overview of 
available testing strategies when using Java Platform Module System (JPMS)
- [Java Best Practices](http://java.jonathangiles.net/)
- [There is no single dependency graph](https://melix.github.io/blog/2022/07/there-is-no-single-dependency-graph.html) -
caveats and misconceptions around resolving application/library dependencies
- [Local Variable Type Inference Style Guidelines](https://openjdk.org/projects/amber/guides/lvti-style-guide) - when to
use (and when not) the `var` keyword
- 📺 [Secrets of Performance Tuning Java on Kubernetes](https://vimeo.com/748031919) - despite the title, it focuses on
the most essential parts like selecting the right GC, defining max heap size, and avoiding CPU throttling
- [GC Causes](https://netflix.github.io/atlas-docs/spectator/lang/java/ext/jvm-gc-causes/) - an useful list of various 
Java garbage collection causes
- [The best way to use Testcontainers with Spring Boot](https://maciejwalkowiak.com/blog/testcontainers-spring-boot-setup/) - the "best"
is always quite subjective, but this one is a really great starting point

## Kotlin

- [Best Practices for Unit Testing in Kotlin](https://phauer.com/2018/best-practices-unit-testing-kotlin/)
- [MockK Guidebook](https://notwoods.github.io/mockk-guidebook/) - a good addition to the official [MockK](https://mockk.io/) 
documentation, especially when it comes to migrating from Mockito
- [Kotlin: An Illustrated Guide](https://typealias.com/start/)

## APIs

- [Zalando RESTful API and Event Guidelines](https://opensource.zalando.com/restful-api-guidelines/)
- [Your Circuit Breaker is Misconfigured](https://shopify.engineering/circuit-breaker-misconfigured) - overview of various
Circuit Breaker parameters and their impact on reliability

## Kafka

- [The Log: What every software engineer should know about real-time data's unifying abstraction](https://engineering.linkedin.com/distributed-systems/log-what-every-software-engineer-should-know-about-real-time-datas-unifying)
- [Turning the database inside-out with Apache Samza](https://martin.kleppmann.com/2015/03/04/turning-the-database-inside-out.html)
- [Squeezing the firehose: getting the most from Kafka compression](https://blog.cloudflare.com/squeezing-the-firehose/) - overview
and comparison of the available message compression methods
- [Optimizing Kafka producers](https://strimzi.io/blog/2020/10/15/producer-tuning/)
- _Exploring Kafka XYZ's Internals_ series
  - [Exploring Kafka Producer’s Internals](https://blog.developer.adobe.com/exploring-kafka-producers-internals-37411b647d0f)
  - [Exploring Kafka Consumer’s Internals](https://medium.com/adobetech/exploring-kafka-consumers-internals-b0b9becaa106)
- 📺 [Kafka: a map of traps for the enlightened dev and op](https://youtu.be/paVdXL5vDzg) - probably the best Kafka deep dive 
I've ever seen (from basic concepts, through operations, and complex "what if X fails?" considerations)

## Databases
- [How a Distributed SQL Database Boosts Secondary Index Queries with Index Only Scan](https://blog.yugabyte.com/how-a-distributed-sql-database-boosts-secondary-index-queries-with-index-only-scan/) - reading 
data directly from the index (PostgreSQL)
- [The Skip Locked feature in Postgres 9.5](https://www.pgcasts.com/episodes/the-skip-locked-feature-in-postgres-9-5) - turning 
PostgreSQL into a simple job queue
- [The What, Why, and When of Single-Table Design with DynamoDB](https://www.alexdebrie.com/posts/dynamodb-single-table/)

## Distributed systems

- [Consistency models](https://jepsen.io/consistency) - a clickable map of relationships between different consistency models
- [Replicated Data Consistency Explained Through Baseball](https://www.microsoft.com/en-us/research/wp-content/uploads/2011/10/ConsistencyAndBaseballReport.pdf)

## Observability

- _Prometheus Range Vectors_ series
  - [Understanding Prometheus Range Vectors](https://satyanash.net/software/2021/01/04/understanding-prometheus-range-vectors.html)
  - [Charting Range Vectors in Prometheus](https://satyanash.net/software/2021/06/09/charting-range-vectors-prometheus.html)
- _How does a Prometheus XYZ work?_ series
  - [How does a Prometheus Counter work?](https://www.robustperception.io/how-does-a-prometheus-counter-work/)
  - [How does a Prometheus Gauge work?](https://www.robustperception.io/how-does-a-prometheus-gauge-work/)
  - [How does a Prometheus Summary work?](https://www.robustperception.io/how-does-a-prometheus-summary-work)
  - [How does a Prometheus Histogram work?](https://www.robustperception.io/how-does-a-prometheus-histogram-work)
- [Awesome Prometheus alerts](https://awesome-prometheus-alerts.grep.to/) - collection of alerting rules for various 
occasions

## Kubernetes

- [In Kubernetes, what should I use as CPU requests and limits?](https://twitter.com/danielepolencic/status/1632717409051181056)
- [A visual guide on troubleshooting Kubernetes deployments](https://learnk8s.io/troubleshooting-deployments)

## Git

- [How to Write a Git Commit Message](https://cbea.ms/git-commit/)
- [A better git blame with --ignore-rev](https://michaelheap.com/git-ignore-rev/) - ignoring certain revisions (e.g. 
code formatting) from `git blame` output

## Software craftsmanship

- [CUPID for joyful coding](https://dannorth.net/2022/02/10/cupid-for-joyful-coding/) - an interesting 
and pragmatic alternative to SOLID (Composable, Unix philosophy, Predictable, Idiomatic, Domain-based)
- [Kent Beck's four rules of simple design](https://martinfowler.com/bliki/BeckDesignRules.html) - passes the tests,
reveals intention, no duplication, fewest elements
- [Safe to fail vs fail safe](https://devskiller.com/techblog/Safe-to-fail-vs-fail-safe/) - unless building a spacecraft,
recovering from failures quickly may be more important than avoiding all possible issues in the first place
- [Exploratory refactoring](https://victorrentea.ro/blog/exploratory-refactoring/) - learning the codebase through
the refactoring
- [The Best Code Review](https://victorrentea.ro/blog/the-best-code-review/) - tips on how to turn code review into
a pleasant, and productive experience
- [20 Things I’ve Learned in my 20 Years as a Software Engineer](https://www.simplethread.com/20-things-ive-learned-in-my-20-years-as-a-software-engineer/) - a handful 
of general tips from an experienced software engineer

## Soft skills & culture

- [The ownership trio](https://alexewerlof.medium.com/the-ownership-trio-482a4e5f666d) - true ownership requires all 3: 
mandate, knowledge, and responsibility
- 📺 [Agility ≠ Speed](https://youtu.be/VnQZ24eeaXM) - what does it really mean to be agile?

## Technical writing

- [The documentation system](https://documentation.divio.com/) - tutorials, how-to guides, explanations, and references
(all serve a different purpose)

## Miscellaneous

- [IDEA - A series of nonverbal algorithm assembly instructions](https://idea-instructions.com/) (IKEA style)
- [Akin's Laws of Spacecraft Design](https://spacecraft.ssl.umd.edu/akins_laws.html)
- [The Difference Between a URL, URI, and URN](https://danielmiessler.com/study/difference-between-uri-url/)
- [Ribbon filter: Practically smaller than Bloom and Xor](https://engineering.fb.com/2021/07/09/data-infrastructure/ribbon-filter/)
- [What you need to know to choose an open source license](https://gist.github.com/nicolasdao/a7adda51f2f185e8d2700e1573d8a633)
- [Wooledge's Bash Guide](https://mywiki.wooledge.org/BashGuide)
