---
title: "About"
date: 2023-05-05T17:21:52+05:30
author: "Devansh Singh"
---

This blog will mainly be composed of my journey in Google Summer of Code 2023. I made a proposal for [Ceph](https://ceph.com/en/), and my project is 'Making Teuthology friendly'.

### Project Overview
[Ceph](https://ceph.com/en/) is an open-sourced software designed storage platform that unifies block, object and file data into a single distributed computer cluster. [Teuthology](https://docs.ceph.com/projects/teuthology/en/latest/README.html) is the integration test framework for Ceph, written in Python. Each set of tests is defined by a *suite* and written as a `.yaml` file. These suites can then be scheduled for a run. In general, it has a bit of a learning curve, and can interrupt the productivity of the team.

My proposal is to implement a REST API and integrate it with [Pulpito](https://pulpito.ceph.com/), which is the dashboard for Ceph test runs and results, so that developers can directly schedule or kill jobs without SSH-ing into Teuthology. The API will be built using [FastAPI](https://fastapi.tiangolo.com/).

### Repositories
The GitHub repositories for the mentioned projects can be found below:

* `Ceph`: https://github.com/ceph/ceph
* `Teuthology`: https://github.com/ceph/teuthology
* `Pulpito`: https://github.com/ceph/pulpito
