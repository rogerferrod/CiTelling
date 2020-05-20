# CiTelling

<b>Structured Semantic Modeling of Citation Intents</b><br>
CiTelling is a radically new model offine-grained semantic structures lying behind citational sentences.
We provide a dataset of citation intents with 1380 instances to be employed within Machine Learning scenarios.

## Getting Started

The project follows an incremental approach, therefore the first step is the construction of a dataset, annotated by hand, containing the information useful for the follwing classification phase.
After a careful analysis of citational intents and meaning, we ended up with five categories (or classes): <i>Analyze, Compare, Extend, Propose and Use.</i> </br>
</br>

To the semantic model we add the concepts of <i>Object</i> and <i>Context</i>, respectively the topic covered by the citation and the context to disambiguate it. In addition, the roles covered by the citation are distinguished: <i>A-subj</i> if the source paper plays the role of subject in presenting the <i>object</i>, <i>B-subj</i> if it the cited paper is the only related to the <i>object</i>. Finally, we subcategorize some classes: <i>Analyze</i> with the subclass <i>'Critique'</i>, <i>Use</i> with <i>'Use-data'</i> and <i>Compare</i> with <i>'Contrast'</i>. Subcategories are indicated through the attribute <i>flags</i>.


### Dataset

The dataset consists of 5 files in csv format, corresponding to the five classes of citations, with values separated by tabs. The first line represents the header.
```
text:       (Peter et al 2019) uses the pm10-2019 dataset for analyze air pollution.
object:     pm10-2018
context:    for analyze air pollution
role:       B-subj
flags:      Data
```


## Authors

* **Roger Ferrod** - [roger.ferrod@unito.it](mailto:roger.ferrod@unito.it)
* **Luigi Di Caro** - [luigi.dicaro@unito.it](mailto:luigi.dicaro@unito.it)
* **Claudio Schifanella** - [claudio.schifanella@unito.it](mailto:claudio.schifanella@unito.it)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

Supervisors:
* Luigi Di Caro
* Claudio Schifanella
