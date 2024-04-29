# Contributing to the human-eval-bia project

Welcome to this page and great to see you are considering to contribute to this project. 
Please note that we have a [code of conduct](CODE-OF-CONDUCT.md) in this project. 
Please follow it to make this a happy community project.

Contributions like feedback, suggestions, notebooks, code, data and pull-requests are very welcome.
It is recommended to open a [github issue](https://github.com/haesleinhuepf/human-eval-bia/issues) 
to discuss things first and make a plan before you spend time and send a pull-request that later cannot be merged because of misunderstandings.

## Aim and scope of this benchmark / test-case collection

We aim at collecting test-cases for benchmarking LLMs for Bio-Image Analysis code generation as wide as possible, but limited to that research field.
Before considering to contribute, please check the following criteria, which serve as guide what we will merge and what not:

We accept:
* new simple or complex tasks commonly done by bio-image analysts
* tasks that can be from any common workflow step in image processing, segmentation, feature extraction, tabular data wranging, statistics, dimensionality reduction, clustering
* tasks that involve multiple example image files or folder (see example_data folder)
* tricky multi-step workflows are explicitly welcome, also if workflow designers suspect that no LLM can solve them at this point.
* tasks for processing imaging modalities such as brightfield microscopy, fluorescence microscopy, electron microscopy, histology/histopathology are welcome
* functional correctness should be evaluated on simple (small) example data, ideally data in the example_data folder is reused

We may not accept:
* new imaging modalities that are not commonly referred to as bio-image analysis (e.g. medical imaging, CT, MRI, astronomy, material science EM)
* new requirements that do not run on common computers or require specific hardware (e.g. CUDA)
* new files in the example_data folder that are larger than few megabytes
* new test-cases that need long run-time (approx > 0.3 seconds)

Out of scope pull-requests are

## Project organization / management

The project is currently maintained and lead by the [benevolent dictator](http://oss-watch.ac.uk/resources/benevolentdictatorgovernancemodel) 
[@haesleinhuepf](https://github.com/haesleinhuepf) who is also open to sharing responsibities. 
If you want to contribute or even become part of the decision making process, please get in touch. 
Everyone is welcome who supports the major aims listed above.

## How contributions become part of the collection

After you submitted a pull-request, it will be reviewed and checked if the conditions above are met. 
We may ask for minor changes and have a discussion about content. We aim at keeping this process short and not wasting anyone's time. 
In case your materials are merged, and your contribution is more than just minor corrections and additions, you will be listed under authors and copyright holders, e.g. in the [LICENSE](LICENSE) file. 
If your affiliation / institution should also be mentioned there, please include this as suggestion in your pull-request.

## Copyright

All contents of this repository are licensed [MIT](LICENSE) by the [authors and contributors](https://github.com/haesleinhuepf/human-eval-bia/contributors), unless mentioned otherwise.
Please make sure your contribution can be shared under the same conditions.

## Changes to these conditions

These conditions may be changed by the maintainers any time. Nothing is nailed in stone. We have to write this to be on the safe side.
If you contributed to the repository earlier and later you are unhappy about your contribution for whatever reasons, 
please send a pull-request removing your contributions. We will accept this pull-request.
