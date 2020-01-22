<p align="center"><img src="https://raw.githubusercontent.com/falcosecurity/community/master/logo/primary-logo.png" width="360"></p>
<p align="center"><b>Cloud Native Runtime Security.</b></p>

<hr>

# The Falco Project

#### Latest release

**v0.18.0**
Read the [change log](https://github.com/falcosecurity/falco/blob/dev/CHANGELOG.md)

Dev Branch: [![Build Status](https://travis-ci.com/falcosecurity/falco.svg?branch=dev)](https://travis-ci.com/falcosecurity/falco)<br />
Master Branch: [![Build Status](https://travis-ci.com/falcosecurity/falco.svg?branch=master)](https://travis-ci.com/falcosecurity/falco)<br />
CII Best Practices: [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/2317/badge)](https://bestpractices.coreinfrastructure.org/projects/2317)

---

Falco is a behavioral activity monitor designed to detect anomalous activity in your applications. Falco audits a system at the most fundamental level, the kernel. Falco then enriches this data with other input streams such as container runtime metrics, and Kubernetes metrics. Falco lets you continuously monitor and detect container, application, host, and network activity—all in one place—from one source of data, with one set of rules.

Falco is hosted by the Cloud Native Computing Foundation (CNCF) as a sandbox level project. If you are an organization that wants to help shape the evolution of technologies that are container-packaged, dynamically-scheduled and microservices-oriented, consider joining the CNCF. For details read the [Falco CNCF project proposal](https://github.com/cncf/toc/tree/master/proposals/falco.adoc).

#### What kind of behaviors can Falco detect?

Falco can detect and alert on any behavior that involves making Linux system calls. Falco alerts can be triggered by the use of specific system calls, their arguments, and by properties of the calling process. For example, Falco can easily detect incidents including but not limited to:

- A shell is running inside a container.
- A container is running in privileged mode, or is mounting a sensitive path, such as `/proc`, from the host.
- A server process is spawning a child process of an unexpected type.
- Unexpected read of a sensitive file, such as `/etc/shadow`.
- A non-device file is written to `/dev`.
- A standard system binary, such as `ls`, is making an outbound network connection.


### Installing Falco

A comprehensive [installation guide](https://falco.org/docs/installation/) for Falco is available in the documentation website.

#### How do you compare Falco with other security tools?

One of the questions we often get when we talk about Falco is “How does Falco differ from other Linux security tools such as SELinux, AppArmor, Auditd, etc.?”. We wrote a [blog post](https://sysdig.com/blog/selinux-seccomp-falco-technical-discussion/) comparing Falco with other tools.


Documentation
---

See [Falco Documentation](https://falco.org/docs/) to quickly get started using Falco.

Join the Community
---

* [Join the mailing list](https://lists.cncf.io/g/cncf-falco-dev/) for news and a Google calendar invite for our Falco open source meetings. Note: this is the only way to get a calendar invite for our open meetings.
* [Website](https://falco.org) for Falco.
* Join our [Public Slack](https://slack.sysdig.com) channel for Falco announcements and discussions.

Community call
---

> Are you using Falco? Do you have have ideas for things to do with Falco? How can Falco be better?

Falco has bi-weekly [community](https://github.com/falcosecurity/community) call which is an open call to discuss Falco from a user perspective. These happen on opposite weeks of Repo planning calls.

[Wednesdays at 8am Pacific](https://lists.cncf.io/g/cncf-falco-dev/calendar) on [Zoom](https://sysdig.zoom.us/j/213235330).

Repo planning
---

> Do you want to contribute to Falco? Are you interested in working on Falco? Do you want to fix something or make something better?

Falco has bi-weekly planning meetings which is an open call to discuss upcoming Falco releases, and assign open GitHub issues to engineers. These happen on opposite weeks of office hours calls.

[Wednesdays at 8am Pacific](https://lists.cncf.io/g/cncf-falco-dev/calendar) on [Zoom](https://sysdig.zoom.us/j/213235330).

License Terms
---

Falco is licensed to you under the [Apache 2.0](./COPYING) open source license.

Contributing
---

See the [CONTRIBUTING.md](./CONTRIBUTING.md).

Security
---

### Security Audit

A third party security audit was performed by Cure53, you can see the full report [here](./audits/SECURITY_AUDIT_2019_07.pdf).

### Reporting security vulnerabilities
Please report security vulnerabilities following the community process documented [here](https://github.com/falcosecurity/.github/blob/master/SECURITY.md).
