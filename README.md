# Resume

## Who is me?

![gyeongil-goo profile](https://avatars2.githubusercontent.com/u/6602501?s=460&v=4)

* Name: Gyeongil-goo 구경일
* Github: https://github.com/yuinacor
* Email: yuiraven@naver.com
* Linkedin: [https://www.linkedin.com/in/%EA%B2%BD%EC%9D%BC-%EA%B5%AC-14150098/](https://www.linkedin.com/in/경일-구-14150098/)



* Open source activities
  * Author
    * [line/gradle-multi-project-support](https://github.com/line/gradle-multi-project-support)
  * Contribute
    * [line/armeria](https://github.com/line/armeria)

> First, solve the problem.
>
> Then, write the code.
>
> - John Johnson

## I can speak

* Korean, Native
* English, Intermediate
* Japanese, Intermediate

## Career

* LINE Plus Corp.
  * 2014.03 ~
  * Backend software developer

## Projects

### LINE Plus Corp.

#### Gradle multi project support

* Author
* 2019.10 ~ 2019.11
* Summary
  * A gradle plugin for support multi project management
  * [Open sourced](https://github.com/line/gradle-multi-project-support)
* Achievement
  * First open source activity further than just contribute
  * [LINE dev day speech](https://youtu.be/32Ttbmg8VLE) in Tokyo
* Technology
  * Gradle
  * Kotlin
  * Git

#### FIDO2 Platform Server

* Project Lead

* 2019.03 ~ 2019.07
* Summary
  * Implement FIDO2 platform for support various FIDO2 based authentication.
* Achievement
  * World first FIDO2 adopted case of Finance industry.
  * Joined FIDO2 Board meeting with this implementation.
  * Understanding about modern crypto protocol.
* Technology
  * FIDO2 specification
  * spring boot2 webflux, reactor
  * Kotlin

#### Bootify and Bootiful

* Project Key Member
* 2019.02 ~ 2019.08
* Summary
  * Modernize legacy spring applications to spring boot.
  * Clarify the way of building reusable spring boot modules.
  * Way of do not reinvent the wheel without any development cost increasing.
* Achievement
  * Team consensus of, **Do not try to solve problems already solved**
  * Team consensus of, **Code reusability**
  * Adopt Kotlin for Bootiful modules
* Technology
  * Unix Philosophy
  * Kotlin
  * Spring boot
  * Spring boot autoconfigure, this called bootiful module

#### Applying CSLB for super high traffic token authentication server

* Project Member
* 2019.05 ~ 2019.12
* Summary
  * CSLB means, Client Side Load Balancing, via service discovery.
  * LINE has open sources, super high performance RPC library named [Armeria](https://github.com/line/armeria) which built over netty, so we adopted it.
  * Originally, this server and client communicate with http2, with L4 load balancer over netty4-beta
  * This project contains two big migration, which is from netty4 to armeria and change the load balancing way from L4 to client side.
  * Main pain point was, http2 uses permanent tcp connection, and L4 just route that connection once then it will be reused, and it means if L7 health check was down, live connection still serves requests. So to handle this point, http2 client side application contains logic for disconnect TCP connection by each duration. This makes too hard to deploy next version, because to cut all incomes, need to L7 down first and wait until that connection disconnected, originally 20 mins, finally 5 mins.
* Achievement
  * Application release time decreased 1 hour to 10 mins.
  * Better latency.
  * Removed one of physical layer which may affect to service quality.
  * More specific route strategy management from client application side.
* Technology
  * netty/armeria
  * Java
  * Asynchronous communication
  * Modern metric collection by prometheus
  * Modern metric visualization by grafana

#### Docker based integrated test environment

* Toy project
* 2019.03 ~ 2019.04
* Summary
  * Make containerized multiple applications over local docker composed private environment, and run test for all over applications
  * Core concept of this project is
    * Run cross over multiple applications in developer's local
    * Give a feedback of one's change so fast
    * Cover multiple repository, different build system
    * Triggered by just one command, no difficult on-demand configuration
* Achievement
  * Developer's own integration test environment
  * Integration test MTTF from 30 min to 5 mins
* Technology
  * Gradle, Kotlin DSL
  * Maven
  * Git submodule
  * Docker
  * Docker-compose

#### Brand new contents platform

* Lead backend developer
* 2017.11 ~ 2018.08
* Summary
  * Brand new contents platform from 0.
  * Various functionalities which will be reused in different new services.
    * Registration, account related functions
    * Authentication, login and session management functions.
    * Follow someone
    * Contents delivery by configured schedule
    * Event delivery for breaking news
    * Multiple dimension category management
    * And so on
  * Co-work with foreign members using English
  * Spread experience of LINE development culture
    * Code review
    * Automated Testing, Auditing...
* Achievement
  * Understand about the real cost of build whole new platfom from 0.
  * Gradle multi project case study
  * Production level docker usage
* Technology
  * Gradle
  * Java
  * Docker
  * Docker orchestration (in house)
  * spring boot

#### App store in LINE service

* Lead Backend developer
* 2017.05 ~ 2017.10
* Summary
  * App in App
  * Design various apis which can interact with LINE chat room.
  * Admin web view, for managing app's
* Achievement
  * From 0 to production
  * Design integration test between multiple projects
* Technology
  * Gradle
  * Java
  * Docker
  * Vue.js/Nuxt.js for admin page
  * spring boot

#### Profile+

* Backend developer
* 2016.01 ~ 2016.11
* Summary
  * Provide user profile information to consumers via iframe based web-view
  * Foggy first plan, and starts with developer side prototyping.
  * Struggled with various security issues.
* Achievement
  * Client/Server side prototyping to make clear goal easy.
* Technology
  * Maven
  * Java

#### Salix -  Suspended

* Key developer
* 2016.06 ~ 2016.08
* Summary
  * FaaS implementation, by composing armeria and centraldogma
  * Write javascript function in centraldogma, and execute it in armeria application
  * Separated execution scope to separate outage
  * Full async io
  * Main requirement was, to support REST(JSON) to Thrift protocol conversion without whole application server deploy.
* Achievement
  * Meaning of java asynchronicity/nio
  * Performance testing for Nashorn script engine in JDK8

* Technology
  * Java
  * Armeria
  * Centraldogma
  * Concept of FaaS
  * Apache Thrift

#### Service Localization Admin

* Frontend/Backend developer
* 2014.10 ~ 2014.11
* Summary
  * Admin tool of managing Service Localization feature of LINE
  * It is similar to A/B testing, has more flexibility.
  * Core logic was designed by senior developer, so focused on admin web page.
* Achievement
  * Understand about planner level requirement
  * Frontend works
* Technology
  * Maven
  * Spring
  * Gulp
  * Angular.js(1.5)
  * Bootstrap
