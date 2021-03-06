# Usage

## How can we use Atomiv for new projects?

The primary intended usage for Atomiv is for building new projects. This is where Atomiv provides the most value - in setting a clean architecture foundation. We recommend the following approach:

1. Install the Atomiv Template via NuGet [https://docs.optivem.com/framework/development/](https://docs.atomiv.com/development) which creates a new Visual Studio solution, with all the layers: Core Layer, Infrastructure Layer, Web Layer, Test Layer
2. Familiarize yourself with the sample code in the generated solution \(bases on the commonly used example in enterprise software - customers, products and orders\), it contains implementation across all layers: Sample REST controllers in the Web Layer, Sample application services and domain entities in the Core Layer, Sample integration with third-party frameworks \(Entity Framework Core, AutoMapper, FluentAssertions, MediatR\) in the Infrastructure Layer, Sample automated tests \(domain unit tests, application service integration tests, REST API integration tests and Selenium system tests\)
3. Based on the sample code, you can starting applying it to your project - i.e. to create relevant REST controllers, application services, domain entities, etc. by following the standardized structure, and when you're comfortable with that you can later delete the sample code
4. In the case that you want to work with additional third-party libraries or replace the default the default third-party libraries included within Atomiv Infrastructure, you can freely do so, by implementing wrappers for any other third-party libraries

_Note: We are also in the process of releasing automated code generation functionality for Atomiv, whereby it will generate classes for your entities across all layers._

## How can we use the Atomiv for existing projects?

A lot of software development revolves in working with existing software systems, by extending them with new features and bug fixing. When working with existing systems, it may be too difficult or risky or expensive to attempt major refactoring or system overhaul, and for that reason we recommend an incremental quality improvement approach using the Atomiv:

1. As a first \(less-invasive\) step, you can use the Atomiv Infrastructure packages individually - using them as you would use other NuGet libraries - with examples as follows: using Atomiv HTTP clients \(based on System.Net\), Csv Serializers \(based on CsvHelper\), Excel readers and writers \(based on EPPlus\), and generic repository and unit of work implementations \(implemented on top of Entity Framework Core 2\) and system utilities \(working with DataTables, reflection, parsing\), and web utilities \(exception handlers, validation responses, CSV formatters for ASP.NET Core\), and automated testing wrappers \(wrappers for automated web testing based on Selenium\)
2. As a next \(more invasive\) step, you can switch to Domain Driven Design \(DDD\) and use-case driven approach by implementing the interfaces from Atomiv Core packages \(Domain and Application\), which would involve refactoring your code into properly separated application services, use cases, entities, value objects, etc.
3. Last, but not least, in cases where changing the existing system is not feasible, we recommend using Atomiv when your team is assigned with the next bigger features or modules - to consider implementing them as microservices, using the Atomiv Template to create the microservice, whereby the old legacy application can communicate with the new microservice, and gradually other parts of the old application may be migrated too

In summary, Atomiv can be used both for new and existing projects - in both cases it will help your team to produce high quality solutions.

## How can Atomiv support our senior developers?

Senior developers often have a key role in the design and architecture of software solutions - whether it's for products, projects, or modules. Aside from that, they are also involved in mentoring and supporting junior developers during development as well as code reviews. From technical perspectives, senior developers are key stakeholders in decisions regarding architecture and quality, building code re-usable, collaboration and knowledge sharing.

At some point in time, as teams and companies grow, they reach a point at which senior developers are not just involved in individual projects, but also in systematizing and standardizing development across the team - which involves often companies producing internal shared code, internal package manager setup, internal samples and templates, etc. based on best practices and coaching team members to push forward adoption. However, this can a time-consuming process, taking months or years to create the adequate code base, yet alone to implement it in practice.

Atomiv can support senior developers so that next time when they need to setup a new project, that they can get it up and running very fast. It also serves to support them in promoting standardization within the teams.

## How can Atomiv support our  junior developers?

Junior developers are an important part of software teams. When junior developers are provided with a solid foundation in software practices and clean code examples, they will be able to contribute with high productivity to software development. This is also an important asset for companies - to be able to grow talent in-house, which can be less expensive and less time-consuming than hiring externally. Over time, these juniors become more experienced and they can mentor and support the next generation of developers.

However, junior developers, a _blank slate_, can be a double-edged sword. On one hand, if junior developers are provided with the right foundation, working on a project which follows best practices, then those juniors can learn by example, and further contribute to the project success. On the other, if junior developers are provided with a poor foundation, working on a project with low quality code, then since this is all they've seen, the poor code will exponentially multiply as the team grows, further decreasing quality and productivity.

This is where Atomiv can help - by providing a template for the entire project architecture and with end-to-end sample working code, developed with best practices in mind, it provides junior developers with practical quality examples so that they can follow the template and apply it for new features and functionalities.

## Next Steps

Are you a Software Architect who wants to build high quality maintainable software architectures?

Are you a Software Developer who wants to write software faster, with less code and higher quality?

Are you a Test Automation Engineer who wants to write automated tests faster and make them easy to maintain?

All the best in your journey towards successful IT projects and products - reach the next level with the Atomiv.

