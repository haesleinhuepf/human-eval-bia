# HumanEval for Bio-image Analysis (HEBIA): Hand-Written Evaluation Set 

This is a fork of the [HumanEval](https://github.com/openai/human-eval) repository where minor modifications were made 
to adapt the evaluation harness for the Bio-image Analysis domain. You find all test cases [listed here](notebooks/human-eval-bia/readme.md)
The original HumanEval repository is an evaluation harness for the HumanEval problem solving dataset described in the paper 
"[Evaluating Large Language Models Trained on Code](https://arxiv.org/abs/2107.03374)".

## Installation

Make sure to use python 3.10 or later:
```
$ mamba create --name heb python=3.10
$ conda activate heb
```

Check out and install this repository:
```
$ git clone https://github.com/haesleinhuepf/human-eval-bia.git
$ cd human-eval-bia
$ pip install -e .
$ pip install -r requirements.txt
```

## Usage

**This program exists to run untrusted model-generated code. Users are strongly
encouraged not to do so outside of a robust security sandbox. The [execution
call](https://github.com/openai/human-eval/blob/master/human_eval/execution.py#L48-L58)
in `execution.py` is deliberately commented out to ensure users read this
disclaimer before running code in a potentially unsafe manner. See the comment in
`execution.py` for more information and instructions.**

![CAUTION]
> Also note when executing the benchmark using commercial models such as chatGPT or gemini, substantial costs can be caused.

To reproduce our benchmarks, you can go through the notebooks provided in the `/notebooks` directory:
* [Create benchmarking test case set from notebooks](notebooks/human-eval-bia/create_cases.ipynb)
* [Create generated code samples from chatGPT/gemini/mistral/codellama/...](notebooks/human-eval-bia/create_samples.ipynb)
* [Evaluate samples by executing code](notebooks/human-eval-bia/evaluate_samples.ipynb)
* [Summarize evaluation](notebooks/human-eval-bia/summarize_evaluation.ipynb)

## Extending the benchmark

You can add new test cases by adding new notebooks to the `/notebooks/human-eval-bia` directory. 
Check out the examples there and make sure to stick to the following rules.

![CAUTION]
> Most importantly: When writing new test case notebooks, do not use language models for code generation. 
> You would otherwise bias the benchmark towards this model. 
> Use human-writen code only and/or examples from the documentation of specific librarires.

The notebooks have to have the following format:
* Within one cell there must be a function that solves a specific [bio-image analysis] task. Very basic example, computing the sum of two numbers:
```python
def sum(a, b):
    """
    This function computes the sum of two numbers.
    """
    return a + b
```
* This function must have a meaningful docstring between """ and """. It must be so meaningful that a language model could possibly write the entire function.
* There must be another code cell that starts with `def check(candiate):` and contains test code to test the generated code.
* The text code must use `assert` statements and call the `candidate` function. E.g. if a given function to test is `sum`, then a valid test for `sum` would be:
```
def check(candidate):
    assert candidate(3, 4) == 7
```
* A third python code cell in the notebook must call the `check` function with your custom function, e.g. like this, to prove that the code you provided works with the tests you wrote:
```
check(sum)
```
* Optional: You can add as many markdown cells as you like to explain the test case.

This is how it works under the hood:
* From the cell with the function definition all code above the docstring, including the docstring, will be stored as prompt. Many prompts from many notebooks will be collected in one `jsonl` file.
* Given language models will be asked to complete the code by adding python code below which does what the docstring claims.
* Afterwards, the generated code examples will be executed and the tests will be run to see if the results were correct.

## Citation

In case you are only using the evaluation code in this repository, consider using and citing [HumanEval](https://github.com/openai/human-eval?tab=readme-ov-file#citation).
If you are using the Bio-image Analysis evaluation set, please cite the following:

```
todo
```
