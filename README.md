## Background

We would like you to prepare a presentation, no longer than twenty
minutes, on approaches to the following problem. This is an active
project that we are working on within the group, so a comprehensive
analysis is beyond our expectations - we're more keen to show you the
sort of question we get asked, and to hear of any suggestions of
approaches you might take.

If you have any difficulties or concerns, please let me know at
gavin.kelly@crick.ac.uk. We will post the responses to any questions
here, so it may be worth checking it again.

We have provided the data as tab-delimited file, so you can analyse
the data with tools of your choosing; if you're under time pressure,
we don't expect a large body of code or slides, we'd much rather that
you consider the issues around such a question.

## The Experiment

Neurons are connected (via long, thin “wires”, called axons). One
neuron receives and sends axons from/to thousands of neurons. Here we
are exclusively labelling input cell (sender) -> target cell
(receiver) connections (unidirectional). Furthermore, as a first
approximation we assume uniform levels of divergence/convergence from
input cells to target cells.

We label neurons in a target area (let’s call them target cells and
the count of them is n<sub>target</sub>) with green colour. As a first
approximation we assume this process is random (but we have control
over how much label we inject, so we can experimentally control
n<sub>target</sub> somewhat). A transformed label (this time with a
red colour) then travels (backwards) to all the upstream connected
neurons (let’s call them input cells, n<sub>input</sub>). We then
extract the brain and count target cells and input cells by simply
counting green and red cells, respectively. There are two different
types of target area A1 and A2; and the experiment is perfomed on mice
of four different genotypes G1...4.

![Scientist's sketch of the setup](sketch.jpg)

![Microscope image of one experiment](real.jpg)

![A cartoon of the brain areas](schematic.jpg)

## The Data

[The data](Data.txt) is a tab-delimited file containing one experiment
per row: the first column labels the type of target area, followed by
a label describing the genotype; then we have the number of target and
input neurons counted in that experiment.

## The Question

From a purely descriptive level, the scientist wants to know how to
describe the relationship between the n<sub>target</sub> measurements and
the corresponding n<sub>input</sub>. Initially we can ignore the
subgroups and see if we can find a good way of describing the
relationship between the target numbers and the corresponding number
of cells in the inputs. They'd then like to know if there are good
ways of parametrising this relationship and, if so, can they use these
to look at possible differences between different genotypes, or
between different target areas.

Ultimately the scientist would like to use these data to build
hypotheses regarding the connectivity between the input and target
areas. Can you think of a mechanistic model that would generate data
of this type, so that rather than a purely empirical approach, we
could start to estimate meaningful parameters about the underlying
mechanisms?


