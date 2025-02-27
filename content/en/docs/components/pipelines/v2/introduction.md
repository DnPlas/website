+++
title = "Introduction"
description = "What is Kubeflow Pipelines?"
weight = 1
                    
+++


Kubeflow Pipelines (KFP) is a platform for building and deploying portable and scalable machine learning (ML) workflows using Docker containers.

With KFP you can author [components][components] and [pipelines][pipelines] using the [KFP Python SDK][pypi], compile pipelines to an [intermediate representation YAML][ir-yaml], and submit the pipeline to run on a KFP-conformant backend such as the [open source KFP backend][oss-be] or [Google Cloud Vertex AI Pipelines](https://cloud.google.com/vertex-ai/docs/pipelines/introduction).

The [open source KFP backend][oss-be] is available as a core component of Kubeflow or as a standalone installation. Follow the [installation][installation] instructions and [Hello World Pipeline][hello-world-pipeline] example to quickly get started with KFP.


<!-- TODO: Include these links once the topic is available -->
<!-- [Learn more about installing Kubeflow][Installation]
[Learn more about installing Kubeflow Pipelines standalone][Installation] -->

## Why Kubeflow Pipelines?
KFP enables data scientists and machine learning engineers to:
* Author end-to-end ML workflows natively in Python
* Create fully custom ML components or leverage an ecosystem of existing components
* Easily manage, track, and visualize pipeline definitions, runs, experiments, and ML artifacts
* Efficiently use compute resources through parallel task execution and through caching to eliminating redundant executions
* Maintain cross-platform pipeline portability through a platform-neutral [IR YAML pipeline definition][ir-yaml]

## What is a pipeline?

A [pipeline][pipelines] is a definition of a workflow that composes one or more [components][components] together to form a computational directed acyclic graph (DAG). At runtime, each component execution corresponds to a single container execution, which may create ML artifacts. Pipelines may also feature [control flow][control-flow].

<!-- TODO: Uncomment these links once the topic is created -->
## Next steps
* [Install KFP][installation]
* Learn more about [authoring components][components]
* Learn more about [authoring pipelines][pipelines]

[components]: /docs/components/pipelines/v2/components
[pipelines]: /docs/components/pipelines/v2/pipelines
[installation]: /docs/components/pipelines/v2/installation
[ir-yaml]: /docs/components/pipelines/v2/compile-a-pipeline#ir-yaml
[oss-be]: /docs/components/pipelines/v2/installation/
<!-- GA TODO: drop /#history tag -->
[pypi]: https://pypi.org/project/kfp/#history
[hello-world-pipeline]: /docs/components/pipelines/v2/hello-world
[control-flow]: /docs/components/pipelines/v2/pipelines/control-flow