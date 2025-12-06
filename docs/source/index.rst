.. _home:

.. raw:: html

   <div class="hero-section">
      <div class="hero-content">
         <h1 class="hero-title">Hyperactive</h1>
         <p class="hero-tagline">A unified interface for optimization algorithms and experiments</p>
      </div>
   </div>

.. raw:: html

   <div class="badge-banner">
      <div class="badge-items">
         <a href="https://pypi.org/project/hyperactive/" target="_blank">
            <img src="https://img.shields.io/pypi/v/hyperactive.svg?style=flat-square&color=5D5D7A" alt="PyPI Version" />
         </a>
         <a href="https://pypi.org/project/hyperactive/" target="_blank">
            <img src="https://img.shields.io/pypi/pyversions/hyperactive.svg?style=flat-square&color=5D5D7A" alt="Python Versions" />
         </a>
         <a href="https://github.com/SimonBlanke/Hyperactive/blob/master/LICENSE" target="_blank">
            <img src="https://img.shields.io/github/license/SimonBlanke/Hyperactive.svg?style=flat-square&color=5D5D7A" alt="License" />
         </a>
         <a href="https://github.com/SimonBlanke/Hyperactive" target="_blank">
            <img src="https://img.shields.io/github/stars/SimonBlanke/Hyperactive?style=flat-square&color=5D5D7A" alt="GitHub Stars" />
         </a>
         <a href="https://gc-os-ai.github.io/" target="_blank">
            <img src="https://img.shields.io/badge/GC.OS-Sponsored-0eac92.svg?style=flat-square" alt="GC.OS Sponsored" />
         </a>
      </div>
   </div>


Hyperactive provides a collection of optimization algorithms, accessible through a unified
experiment-based interface that separates optimization problems from algorithms. The library
provides native implementations of algorithms from the Gradient-Free-Optimizers package
alongside direct interfaces to Optuna and scikit-learn optimizers.

----

Why Hyperactive?
================

.. grid:: 1 2 3 3
   :gutter: 4

   .. grid-item-card::
      :class-card: feature-card

      **20 Optimization Algorithms**
      ^^^
      From Hill Climbing to Bayesian Optimization,
      Particle Swarm, Genetic Algorithms, and more.

      +++
      Local, global, population-based, and sequential methods.

   .. grid-item-card::
      :class-card: feature-card

      **Direct ML Integration**
      ^^^
      First-class support for scikit-learn, sktime, skpro, and PyTorch.
      Tune models with minimal code changes.

      +++
      Works with any estimator implementing fit/score.

   .. grid-item-card::
      :class-card: feature-card

      **Experiment Abstraction**
      ^^^
      Clean separation between *what* to optimize (experiments) and
      *how* to optimize (algorithms).

      +++
      Swap algorithms without changing experiment code.

   .. grid-item-card::
      :class-card: feature-card

      **3 Optimizer Backends**
      ^^^
      Native GFO algorithms, Optuna samplers, and scikit-learn
      search methods through one unified API.

      +++
      GFO · Optuna · sklearn

   .. grid-item-card::
      :class-card: feature-card

      **Mixed Parameter Spaces**
      ^^^
      Categorical, integer, and continuous parameters.
      Define search spaces with NumPy arrays or lists.

      +++
      Optuna backend supports native continuous ranges.

   .. grid-item-card::
      :class-card: feature-card

      **Stable Since 2019**
      ^^^
      5+ years of development, comprehensive test coverage,
      and active maintenance.

      +++
      Type-annotated · Documented · Tested

----

Quick Example
=============

Get started in just a few lines of code:

.. tab-set::

   .. tab-item:: Custom Function

      .. literalinclude:: _snippets/getting_started/index_custom_function.py
         :language: python
         :start-after: # [start:full_example]
         :end-before: # [end:full_example]

   .. tab-item:: Scikit-learn Tuning

      .. literalinclude:: _snippets/getting_started/index_sklearn_tuning.py
         :language: python
         :start-after: # [start:full_example]
         :end-before: # [end:full_example]

   .. tab-item:: Bayesian Optimization

      .. literalinclude:: _snippets/getting_started/index_bayesian.py
         :language: python
         :start-after: # [start:full_example]
         :end-before: # [end:full_example]

----

.. raw:: html

   <div class="visualization-section">
      <h2>Visualization</h2>
      <p>Watch Bayesian Optimization intelligently explore parameter space:</p>
      <img src="_static/images/bayes_convex.gif" alt="Bayesian Optimization Animation" class="optimization-gif" />
   </div>

----

Available Algorithms
====================

.. grid:: 1 2 2 4
   :gutter: 3

   .. grid-item-card::
      :class-card: algo-card

      **Local Search**
      ^^^
      - Hill Climbing
      - Repulsing Hill Climbing
      - Simulated Annealing
      - Downhill Simplex

   .. grid-item-card::
      :class-card: algo-card

      **Global Search**
      ^^^
      - Random Search
      - Grid Search
      - Random Restart Hill Climbing
      - Powell's Method
      - Pattern Search

   .. grid-item-card::
      :class-card: algo-card

      **Population Methods**
      ^^^
      - Parallel Tempering
      - Particle Swarm
      - Spiral Optimization
      - Genetic Algorithm
      - Evolution Strategy
      - Differential Evolution

   .. grid-item-card::
      :class-card: algo-card

      **Sequential / Bayesian**
      ^^^
      - Bayesian Optimization
      - Tree-Parzen Estimators
      - Forest Optimizer
      - Lipschitz Optimization
      - DIRECT Algorithm

.. grid:: 1 2 2 4
   :gutter: 3

   .. grid-item-card::
      :class-card: algo-card optuna-card

      **Optuna Backend**
      ^^^
      - TPE Optimizer
      - CMA-ES
      - Gaussian Process
      - NSGA-II / NSGA-III
      - QMC Optimizer

----

Integrations
============

.. grid:: 1 2 4 4
   :gutter: 4

   .. grid-item::
      :class: integration-item

      .. raw:: html

         <div class="integration-card">
            <div class="integration-name">scikit-learn</div>
            <div class="integration-desc">Cross-validation experiments</div>
         </div>

   .. grid-item::
      :class: integration-item

      .. raw:: html

         <div class="integration-card">
            <div class="integration-name">sktime</div>
            <div class="integration-desc">Time series forecasting</div>
         </div>

   .. grid-item::
      :class: integration-item

      .. raw:: html

         <div class="integration-card">
            <div class="integration-name">skpro</div>
            <div class="integration-desc">Probabilistic regression</div>
         </div>

   .. grid-item::
      :class: integration-item

      .. raw:: html

         <div class="integration-card">
            <div class="integration-name">PyTorch</div>
            <div class="integration-desc">Deep learning models</div>
         </div>

----

Quick Install
=============

.. code-block:: bash

   pip install hyperactive

For additional integrations:

.. code-block:: bash

   # Full installation with all extras
   pip install hyperactive[all_extras]

   # Or specific integrations
   pip install hyperactive[sklearn-integration]
   pip install hyperactive[sktime-integration]

----

Contents
========

.. toctree::
   :maxdepth: 1
   :hidden:

   get_started
   installation
   user_guide
   api_reference
   examples
   faq
   troubleshooting
   get_involved
   about

.. grid:: 1 2 2 3
   :gutter: 3

   .. grid-item-card::
      :text-align: center
      :class-card: nav-card

      :fas:`rocket` **Get Started**
      ^^^

      Quick introduction to using Hyperactive.

      +++

      .. button-ref:: get_started
         :color: primary
         :click-parent:
         :expand:

         Get Started

   .. grid-item-card::
      :text-align: center
      :class-card: nav-card

      :fas:`download` **Installation**
      ^^^

      Installation guide and requirements.

      +++

      .. button-ref:: installation
         :color: primary
         :click-parent:
         :expand:

         Installation

   .. grid-item-card::
      :text-align: center
      :class-card: nav-card

      :fas:`book` **User Guide**
      ^^^

      In-depth tutorials and explanations.

      +++

      .. button-ref:: user_guide
         :color: primary
         :click-parent:
         :expand:

         User Guide

   .. grid-item-card::
      :text-align: center
      :class-card: nav-card

      :fas:`code` **API Reference**
      ^^^

      Technical reference for all classes.

      +++

      .. button-ref:: api_reference
         :color: primary
         :click-parent:
         :expand:

         API Reference

   .. grid-item-card::
      :text-align: center
      :class-card: nav-card

      :fas:`laptop-code` **Examples**
      ^^^

      Code examples and use cases.

      +++

      .. button-ref:: examples
         :color: primary
         :click-parent:
         :expand:

         Examples

   .. grid-item-card::
      :text-align: center
      :class-card: nav-card

      :fas:`users` **Get Involved**
      ^^^

      Contribute to Hyperactive.

      +++

      .. button-ref:: get_involved
         :color: primary
         :click-parent:
         :expand:

         Get Involved
