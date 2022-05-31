## Database as Code. Not only migrations

Hey! My name is Maks. I am independent database consultant and big fun of SQL. And today we gonna talk about "Database as Code" topic.
- What is it?
- Is there it in real life?
- And we will see that migration scripts are just the very beginning of the hard road to "Database as Code"



### Everything as Code

Let's start from the very beginning, specifically from "Everything as Code" things.

The DevOps era brought to us "Everything as Code" philosophy, where any IT area might be represented as a plain code, and we can work with it using standard tools and technologies (code editors, control version systems, static anlyzys, CI/CD pipelines etc.). And yes, indeed, there are many "Everything as Code" realizations for many areas, for example:

- Pipeline as Code (`Jenkinsfile`, `.gitlab-ci.yml`, `settings.kts` in TeamCity)
- Infrastructure as Code (Kubernetes, Terraform, Ansible)
- Diagram as Сode (PlantUML, Graphviz, Mermaid)
- Documentation as Сode (Markdown, AsciiDoc)
- Tests as Code (Gatling, Cucumber)
- And things like that

### Everything as Code. Pros

We are used to the everything as code things

- No Monstrous GUI - where you are afraid to click something wrong
- Version control - who, where and when do something
- Review
- Testing



### Everybody ~Lies~ is Coding

And as a result we have had a unique situation - everybody is coding.

- Developers
- Testers
- Engineers
- Analysts

And have many common languages for everyone:
- yml
- json
- xml
- toml

And it's great!

### Database as Code

But how about "Database as Code"? It was still a very exotic combination of words, and Dan North offers four simple rules for treating a database like Code:

- All changes scripted and automated
- All changes under version control
- Ability to release on demand
- DBA's integrated with Dev and Ops

It's been six years, and nowadays, it's hard to find a project that doesn't follow these rules (at least the first three). There are a lot of different database migration tools and different ways to integrate it with your VCS and your CI/CD pipeline. And it's really great.

- Flyway
- gh-ost
- Sqitch
- Skeema
- Bytebase

And Liquibase ofcourse

But for now its associates mostly with database schema changes.



### Database is not only schema changes

- Queries
- Administration
- Monitoring
- Documentation


### SQL

But in dabases World we already have great universal language with marvelous history, and it is SQL.

SQL allows you standatizied declarative access not only to relational DB, but to non relational DB, streaming, files, cloud inventory and etc

In nowaday we use SQL everywhere - in traditional relational system (like PostgreSQL and MySQL), in non-relational (Cassandra, Tarantool) in analytical systems (like Snowflake, ClickHouse), in streaming platforms (like Kafka and Flink) in сloud infrastructure (Steampipe, Resmo, CloudQuery)

- Relational DB
- Non-Relational DB
- Analytical DB
- Streaming Platforms
- Сloud



### SQL Hell

Like a DLL hell or JAR hell

- generated queries
- queries injected in another code like literals
- queries in config files of variuous systems
- different versions

- Generated Queries
- injected Queries
- Queries in config files
- Different versions


And its nightmare
- we have not single point
- we have not review
- we have not testing


### Keep SQL as Plain Code

Its very simple idea i think, just put your sql queries into your git repo, as plain sql files.

For what?
- sql is a code
- Query its a value, All another (web, json, etc) is a boilerplate code

benefits :
- pipeline
- common tools


### Is There It in WildLife?

And finally lets look


https://twitter.com/pedram_navid/status/1514080871103356929?t=6eSGcCrQGmFUdraif61pJg&s=19



And lets try create more database as code tools together!
