:github_url: https://github.com/pytorch/torchx

TorchX
==================

TorchX is a universal job launcher for PyTorch applications.
TorchX is designed to have fast iteration time for training/research and support
for E2E production ML pipelines when you're ready.

**GETTING STARTED?** Follow the :ref:`quickstart guide<quickstart:Quickstart>`.


In 1-2-3
-----------------

Step 1. Install

.. code-block:: shell

   pip install torchx[dev]

Step 2. Run Locally

.. code-block:: shell

   torchx run --scheduler local_cwd utils.python --script my_app.py "Hello, localhost!"

Step 3. Run Remotely

.. code-block:: shell

   torchx run --scheduler kubernetes utils.python --script my_app.py "Hello, Kubernetes!"


Documentation
---------------

.. toctree::
   :maxdepth: 1
   :caption: Usage

   quickstart.md
   cli
   basics
   runner.config
   advanced
   custom_components.md


Works With
---------------

.. _Schedulers:
.. toctree::
   :maxdepth: 1
   :caption: Schedulers

   schedulers/local
   schedulers/docker
   schedulers/kubernetes
   schedulers/slurm
   schedulers/ray
   schedulers/aws_batch

.. _Pipelines:
.. toctree::
   :maxdepth: 1
   :caption: Pipelines

   pipelines/kfp


Examples
------------

.. toctree::
   :maxdepth: 1
   :caption: Examples


   examples_apps/index
   examples_pipelines/index



Components Library
---------------------
.. _Components:
.. toctree::
   :maxdepth: 1
   :caption: Components

   components/overview
   components/train
   components/distributed
   components/interpret
   components/metrics
   components/hpo
   components/serve
   components/utils

Runtime Library
----------------
.. toctree::
   :maxdepth: 1
   :caption: Application (Runtime)

   runtime/overview
   runtime/hpo
   runtime/tracking


Reference
-----------

.. _torchx.api:
.. toctree::
   :maxdepth: 1
   :caption: API

   specs
   runner
   schedulers
   workspace
   pipelines

.. toctree::
   :maxdepth: 1
   :caption: Best Practices

   app_best_practices
   component_best_practices
