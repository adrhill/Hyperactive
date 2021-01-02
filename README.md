<p align="center">
  <br>
  <a href="https://simonblanke.github.io/Hyperactive/"><img src="./docs/images/logo.png" height="200"></a>
  <br>
</p>

<br>

---

<h2 align="center">A hyperparameter optimization and meta-learning toolbox for convenient and fast prototyping of machine-learning models.</h2>

<br>

<table>
  <tbody>
    <tr align="left" valign="center">
      <td>
        <strong>Master status:</strong>
      </td>
      <td>
        <a href="https://travis-ci.com/SimonBlanke/Hyperactive">
          <img src="https://img.shields.io/travis/com/SimonBlanke/Hyperactive/master?style=flat-square&logo=travis" alt="img not loaded: try F5 :)">
        </a>
        <a href="https://coveralls.io/github/SimonBlanke/Hyperactive">
          <img src="https://img.shields.io/coveralls/github/SimonBlanke/Hyperactive?style=flat-square&logo=codecov" alt="img not loaded: try F5 :)">
        </a>
      </td>
    </tr>
    <tr/>
    <tr align="left" valign="center">
      <td>
        <strong>Dev status:</strong>
      </td>
      <td>
        <a href="https://travis-ci.com/SimonBlanke/Hyperactive">
          <img src="https://img.shields.io/travis/SimonBlanke/Hyperactive/dev?style=flat-square&logo=travis" alt="img not loaded: try F5 :)">
        </a>
        <a href="https://coveralls.io/github/SimonBlanke/Hyperactive?branch=dev">
          <img src="https://img.shields.io/coveralls/github/SimonBlanke/Hyperactive/dev?style=flat-square&logo=codecov" alt="img not loaded: try F5 :)">
        </a>
      </td>
    </tr>
    <tr/>    <tr align="left" valign="center">
      <td>
         <strong>Code quality:</strong>
      </td>
      <td>
        <a href="https://codeclimate.com/github/SimonBlanke/Hyperactive">
        <img src="https://img.shields.io/codeclimate/maintainability/SimonBlanke/Hyperactive?style=flat-square&logo=code-climate" alt="img not loaded: try F5 :)">
        </a>
        <a href="https://scrutinizer-ci.com/g/SimonBlanke/Hyperactive/">
        <img src="https://img.shields.io/scrutinizer/quality/g/SimonBlanke/Hyperactive?style=flat-square&logo=scrutinizer-ci" alt="img not loaded: try F5 :)">
        </a>
      </td>
    </tr>
    <tr/>    <tr align="left" valign="center">
      <td>
        <strong>Latest versions:</strong>
      </td>
      <td>
        <a href="https://github.com/SimonBlanke/Hyperactive/releases">
          <img src="https://img.shields.io/github/v/release/SimonBlanke/Hyperactive?style=flat-square&logo=github" alt="img not loaded: try F5 :)">
        </a>
        <a href="https://pypi.org/project/hyperactive/">
          <img src="https://img.shields.io/pypi/v/Hyperactive?style=flat-square&logo=PyPi&logoColor=white" alt="img not loaded: try F5 :)">
        </a>
      </td>
    </tr>
  </tbody>
</table>

<br>

NEWS:

Hyperactive is currently in a transition phase between version 2 and 3. All of the source code for the optimization algorithms will be stored in <a href="https://github.com/SimonBlanke/Gradient-Free-Optimizers">Gradient-Free-Optimizers</a>. Gradient-Free-Optimizers will serve as an easy to use stand alone package as well as the optimization backend for Hyperactive in the future. Until Hyperactive version 3 is released you can either switch to the 2.x.x branch for the old version in Github or use Gradient-Free-Optimizers to enjoy new algorithms and improved performance.



<br>

Hyperactive is primarly a <b>hyperparameter optimization toolkit</b>, that aims to simplify the model-selection and -tuning process. You can use any machine- or deep-learning package and it is not necessary to learn new syntax. Hyperactive offers <b>high versatility</b> in model optimization because of two characteristics:

  - You can define any kind of model in the objective function. It just has to return a score/metric that gets maximized.
  - The search space accepts not just 'int', 'float' or 'str' as data types but even functions, classes or any python objects.


<br>

---

<div align="center"><a name="menu"></a>
  <h3>
    <a href="https://github.com/SimonBlanke/Hyperactive#main-features">Main features</a> •
    <a href="https://github.com/SimonBlanke/Hyperactive#installation">Installation</a> •
    <a href="https://github.com/SimonBlanke/Hyperactive#roadmap">Roadmap</a> •
    <a href="https://github.com/SimonBlanke/Hyperactive#citing-hyperactive">Citation</a> •
    <a href="https://github.com/SimonBlanke/Hyperactive#license">License</a>
  </h3>
</div>

---

<br>



Hyperactive features a collection of optimization algorithms that can be used for a variety of optimization problems. The following table shows listings of the capabilities of Hyperactive, where each of the items links to an example:

<table>
  <tbody>
    <tr align="center" valign="center">
      <td>
        <strong>Optimization Techniques</strong>
        <img src="./docs/images/blue.jpg"/>
      </td>
      <td>
        <strong>Tested and Supported Packages</strong>
        <img src="./docs/images/blue.jpg"/>
      </td>
      <td>
        <strong>Optimization Applications</strong>
        <img src="./docs/images/blue.jpg"/>
      </td>
    </tr>
    <tr/>
    <tr valign="top">
      <td>
        <a><b>Local Search:</b></a>
          <ul>
            <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/optimization_techniques/hill_climbing.py">Hill Climbing</a></li>
            <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/optimization_techniques/repulsing_hill_climbing.py">Repulsing Hill Climbing</a></li>
            <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/optimization_techniques/simulated_annealing.py">Simulated Annealing</a></li>
         </ul><br>
        <a><b>Global Search:</b></a>
          <ul>
            <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/optimization_techniques/random_search.py">Random Search</a></li>
            <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/optimization_techniques/rand_rest_hill_climbing.py">Random Restart Hill Climbing</a></li>
            <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/optimization_techniques/random_annealing.py">Random Annealing</a> [<a href="#/./overview#experimental-algorithms">*</a>] </li>
         </ul><br>
        <a><b>Population Methods:</b></a>
          <ul>
            <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/optimization_techniques/parallel_tempering.py">Parallel Tempering</a></li>
            <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/optimization_techniques/particle_swarm_optimization.py">Particle Swarm Optimizer</li>
            <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/optimization_techniques/evolution_strategy.py">Evolution Strategy</a></li>
          </ul><br>
        <a><b>Sequential Methods:</b></a>
          <ul>
            <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/optimization_techniques/bayesian_optimization.py">Bayesian Optimization</a></li>
            <li><a href="https://simonblanke.github.io/Hyperactive/#/./optimizers/sequential_mehttps://github.com/SimonBlanke/Hyperactive/tree/master/examples/optimization_techniques/tpe.py">Tree of Parzen Estimators</a></li>
            <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/optimization_techniques/decision_tree_optimization.py">Decision Tree Optimizer</a>
            [<a href="#/./overview#references">dto</a>] </li>
          </ul>
      </td>
      <td>
        <a><b>Machine Learning:</b></a>
          <ul>
              <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/tested_and_supported_packages/sklearn_example.py">Scikit-learn</a></li>
              <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/tested_and_supported_packages/xgboost_example.py">XGBoost</a></li>
              <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/tested_and_supported_packages/lightgbm_example.py">LightGBM</a></li>
              <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/tested_and_supported_packages/catboost_example.py">CatBoost</a></li>
              <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/tested_and_supported_packages/rgf_example.py">RGF</a></li>
              <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/tested_and_supported_packages/mlxtend_example.py">Mlxtend</a></li>
          </ul><br>
        <a><b>Deep Learning:</b></a>
          <ul>
              <li>Tensorflow</li>
              <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/tested_and_supported_packages/keras_example.py">Keras</a></li>
              <li>Pytorch</li>
          </ul><br>
        <a><b>Parallel Computing:</b></a>
          <ul>
              <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/tested_and_supported_packages/multiprocessing_example.py">Multiprocessing</a></li>
              <li>Joblib</li>
          </ul>
      </td>
      <td>
        <a><b>Feature Engineering:</b></a>
          <ul>
            <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/optimization_applications/feature_transformation.py">Feature Transformation</a></li>
            <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/optimization_applications/feature_selection.py">Feature Selection</a></li>
            <li>Feature Construction</li>
          </ul>
        <a><b>Machine Learning:</b></a>
          <ul>
            <li>Hyperparameter Tuning/li>
            <li>Model Selection</li>
            <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/optimization_applications/sklearn_pipeline_example.py">Sklearn Pipelines</a></li>
            <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/optimization_applications/ensemble_learning_example.py">Ensemble Learning</a></li>
          </ul>
        <a><b>Deep Learning:</b></a>
          <ul>
            <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/optimization_applications/neural_architecture_search.py">Neural Architecture Search</a></li>
            <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/optimization_applications/enas.py">Efficient Neural Architecture Search</a></li>
            <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/optimization_applications/transfer_learning.py">Transfer Learning</a></li>
          </ul>
        <a><b>Meta-data:</b></a>
          <ul>
            <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/optimization_applications/meta_data_collection.py">Meta-data Collection</a></li>
            <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/optimization_applications/meta_optimization.py">Meta Optimization</a></li>
            <li><a href="https://github.com/SimonBlanke/Hyperactive/tree/master/examples/optimization_applications/meta_learning.py">Meta Learning</a></li>
          </ul>
        <a><b>Miscellaneous:</b></a>
          <ul>
            <li>Test Functions</li>
            <li>Fit Gaussian Curves</li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

<br>

## Installation
[![PyPI version](https://badge.fury.io/py/hyperactive.svg)](https://badge.fury.io/py/hyperactive)

The most recent version of Hyperactive is available on PyPi:
```console
pip install hyperactive
```

<br>

## Minimal example

```python
from sklearn.model_selection import cross_val_score
from sklearn.ensemble import GradientBoostingRegressor
from sklearn.datasets import load_boston
from hyperactive import Hyperactive

data = load_boston()
X, y = data.data, data.target

""" define the model in a function """
def model(opt):
    """ pass the suggested parameter to the machine learning model """
    gbr = GradientBoostingRegressor(
        n_estimators=opt["n_estimators"]
    )
    scores = cross_val_score(gbr, X, y, cv=3)

    """ return a single numerical value, which gets maximized """
    return scores.mean()


""" 
create the search space 
determines the ranges of parameters you want the optimizer to search through
"""
search_space = {"n_estimators": list(range(10, 200, 5))}

""" start the optimization run """
hyper = Hyperactive()
hyper.add_search(model, search_space, n_iter=50)
hyper.run()
```


## Hyperactive API information

<details>
<summary><b> Hyperactive(...)</b></summary>

    - verbosity = ["progress_bar", "print_results", "print_times"]
    - distribution = {"multiprocessing": {"initializer": tqdm.set_lock, "initargs": (tqdm.get_lock(),),}}

</details>


<details>
<summary><b> .add_search(...)</b></summary>

    - model
    - search_space
    - n_iter
    - optimizer = RandomSearchOptimizer()
    - n_jobs = 1
    - initialize = {"grid": 4, "random": 2, "vertices": 4}
    - max_score = None
    - random_state = None
    - memory = True
    - memory_warm_start = None

</details>


<details>
<summary><b> .run(...)</b></summary>

    - max_time = None

</details>


### Optimizers

<details>
<summary><b> HillClimbingOptimizer</b></summary>

    - epsilon=0.05
    - distribution="normal"
    - n_neighbours=3
    - rand_rest_p=0.03

</details>

<details>
<summary><b> RepulsingHillClimbingOptimizer</b></summary>

    - epsilon=0.05
    - distribution="normal"
    - n_neighbours=3
    - rand_rest_p=0.03
    - repulsion_factor=3

</details>

<details>
<summary><b> SimulatedAnnealingOptimizer</b></summary>

    - epsilon=0.05
    - distribution="normal"
    - n_neighbours=3
    - rand_rest_p=0.03
    - p_accept=0.1
    - norm_factor="adaptive"
    - annealing_rate=0.975
    - start_temp=1

</details>

<details>
<summary><b> RandomSearchOptimizer</b></summary>

</details>

<details>
<summary><b> RandomRestartHillClimbingOptimizer</b></summary>

    - epsilon=0.05
    - distribution="normal"
    - n_neighbours=3
    - rand_rest_p=0.03
    - n_iter_restart=10

</details>

<details>
<summary><b> RandomAnnealingOptimizer</b></summary>

    - epsilon=0.05
    - distribution="normal"
    - n_neighbours=3
    - rand_rest_p=0.03
    - annealing_rate=0.975
    - start_temp=1

</details>

<details>
<summary><b> ParallelTemperingOptimizer</b></summary>

    - n_iter_swap=10
    - rand_rest_p=0.03

</details>

<details>
<summary><b> ParticleSwarmOptimizer</b></summary>

    - inertia=0.5
    - cognitive_weight=0.5
    - social_weight=0.5
    - temp_weight=0.2
    - rand_rest_p=0.03

</details>

<details>
<summary><b> EvolutionStrategyOptimizer</b></summary>

    - mutation_rate=0.7
    - crossover_rate=0.3
    - rand_rest_p=0.03

</details>

<details>
<summary><b> BayesianOptimizer</b></summary>

    - gpr=gaussian_process["gp_nonlinear"]
    - xi=0.03
    - warm_start_smbo=None
    - rand_rest_p=0.03

</details>

<details>
<summary><b> TreeStructuredParzenEstimators</b></summary>

    - gamma_tpe=0.5
    - warm_start_smbo=None
    - rand_rest_p=0.03

</details>

<details>
<summary><b> DecisionTreeOptimizer</b></summary>

    - tree_regressor="extra_tree"
    - xi=0.01
    - warm_start_smbo=None
    - rand_rest_p=0.03

</details>






<br>

## Roadmap

<details>
<summary><b>v2.0.0</b>:heavy_check_mark:</summary>

  - [x] Change API
</details>

<details>
<summary><b>v2.1.0</b>:heavy_check_mark:</summary>

  - [x] Save memory of evaluations for later runs (long term memory)
  - [x] Warm start sequence based optimizers with long term memory
  - [x] Gaussian process regressors from various packages (gpy, sklearn, GPflow, ...) via wrapper
</details>

<details>
<summary><b>v2.2.0</b>:heavy_check_mark:</summary>

  - [x] Add basic dataset meta-features to long term memory
  - [x] Add helper-functions for memory
      - [x] connect two different model/dataset hashes
      - [x] split two different model/dataset hashes
      - [x] delete memory of model/dataset
      - [x] return best known model for dataset
      - [x] return search space for best model
      - [x] return best parameter for best model
</details>

<details>
<summary><b>v2.3.0</b>:heavy_check_mark:</summary>

  - [x] Tree-structured Parzen Estimator
  - [x] Decision Tree Optimizer
  - [x] add "max_sample_size" and "skip_retrain" parameter for sbom to decrease optimization time
</details>

<details open>
<summary><b>v3.0.0</b></summary>

  - [x] New API
      - [x] expand usage of objective-function
      - [x] No passing of training data into Hyperactive
      - [x] Removing "long term memory"-support (better to do in separate package)
      - [x] More intuitive selection of optimization strategies and parameters
      - [x] Separate optimization algorithms into other package
      - [x] expand api so that optimizer parameter can be changed at runtime
      - [x] add extensive testing procedure (similar to Gradient-Free-Optimizers)

</details>


<br>



## Experimental algorithms

The following algorithms are of my own design and, to my knowledge, do not yet exist in the technical literature.
If any of these algorithms already exist I would like you to share it with me in an issue.

#### Random Annealing

A combination between simulated annealing and random search.


<br>

## References

#### [dto] [Scikit-Optimize](https://github.com/scikit-optimize/scikit-optimize/blob/master/skopt/learning/forest.py)

<br>

## Citing Hyperactive

    @Misc{hyperactive2019,
      author =   {{Simon Blanke}},
      title =    {{Hyperactive}: A hyperparameter optimization and meta-learning toolbox for machine-/deep-learning models.},
      howpublished = {\url{https://github.com/SimonBlanke}},
      year = {since 2019}
    }


<br>

## License

[![LICENSE](https://img.shields.io/github/license/SimonBlanke/Hyperactive?style=for-the-badge)](https://github.com/SimonBlanke/Hyperactive/blob/master/LICENSE)
