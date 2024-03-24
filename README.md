# HumanEval for Bio-image Analysis (HEBIA): Hand-Written Evaluation Set 

This is a fork of the [HumanEval](https://github.com/openai/human-eval) repository where minor modifications were made 
to adapt the evaluation harness for the Bio-image Analysis domain. 
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

To reproduce our benchmarks, you can go through the notebooks provided in the `/notebooks` directory:
* [Create benchmarking test case set from notebooks](notebooks/create_cases.ipynb)
* [Create generated code samples from chatGPT/gemini/mistral/codellama/...](notebooks/create_samples.ipynb)
* [Evaluate samples by executing code](notebooks/evaluate_samples.ipynb)
* [Summarize evaluation](notebooks/summarize_evaluation.ipynb)


## Citation

In case you are only using the evaluation code in this repository, consider using and citing [HumanEval](https://github.com/openai/human-eval?tab=readme-ov-file#citation).
If you are using the Bio-image Analysis evaluation set, please cite the following:

```
todo
```
