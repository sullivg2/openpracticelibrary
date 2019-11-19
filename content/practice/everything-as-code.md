---
title: Everything-as-Code
subtitle: 'Save everything as code - configuration, infrastructure and pipelines.'
date: '2018-08-15T10:37:16+01:00'
authors:
  - springdo
  - makentenza
  - Zenigata
area: foundation-technical
icon: /images/ansible-example.png
people: ''
participants: []
---
## What is it?

Everything as Code is the practice of treating all parts of the system as code. This means storing configuration along with Source Code in a repository such as [Git](https://git-scm.com/) or [SVN](https://subversion.apache.org/).

Storing the configuration from bottom to top (communication switches, bare metal servers, operating systems, build configurations, application properties and deployment configurations...) as code means they are tracked and can be recreated at the click of a button.

Everything-as-Code includes system design, also stored as code. In old world IT, infrastructure required specialised skills, physical hardware and cables to be installed. Systems were precious or were not touched or updated often as the people who created them no longer worked for the company. The dawn of cloud computing and cloud native applications has meant it is cheap and easy to spin up virtual infrastructure. By storing the configuration of virtual environments as code, they can be life-cycled and recreated whenever needed.

## Why store all things as code?

1. **Traceability** - Storing your config in `git` implies that controls are in place to track who or why a config has changed. Changes can then be applied and reverted, they are tracked to a single user who made the change.
2. **Repeatability** - Moving from one cloud provider to another should be simple in modern application development. Picking a deployment target should be like shopping around for the current best price. By storing all things as code, systems can be re-created in moments in various providers.
3. **Test** - Infra and code can be rolled out, validated and promoted into production environments with confidence and assurance that they will behave as expected.
4. **Phoenix server** - No more fear of a servers' configuration drifting. If a server needs to be patched or randomly dies, it's OK. Just create it again from the stored configuration.
5. **Shared understanding** - When a cross-functional team is using 'Everything-as-Code' to describe all the parts of the product, they are developing together, i.e. they contribute to increase the shared understanding between Developers and Operations, they speak the same language to describe the state of this product, and they use the same frameworks to accomplish their goals.

## Further reading

* Martin Fowler on [Infra as Code](https://martinfowler.com/bliki/InfrastructureAsCode.html).
* [Ansible](https://www.ansible.com/) is an infrastructure automation tool created by Red Hat, the huge enterprise open source technology provider.
