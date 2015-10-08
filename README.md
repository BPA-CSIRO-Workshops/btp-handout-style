We suggest that you do not use this repository directly unless you know what you are doing. Instead, you should 
probably head over to the [btp-workshop-template](https://github.com/BPA-CSIRO-Workshops/btp-workshop-template)
repository and follow one of the
[workflows](https://github.com/BPA-CSIRO-Workshops/btp-workshop-template#general-workflows) documented there.

Table of Contents
=================
<!-- toc -->
* [Overview](#overview)
* [Usage](#usage)
* [Commands](#commands)
* [Paragraph Text Environments](#paragraph-text-environments)

<!-- toc stop -->

Overview
========

This repository provides a LaTeX style file for use with creating consistently styled workshop excercise handouts. It
should be included as a submodule at the level of a BTP workshop repository. This is so that any workshop modules,
included as submodules in that workshop repository, have access to it.

What follows are details about the features available through the use of this LaTeX package.

Usage
=====

Include the BTP package in your LaTeX project to generate the trainee version of the handout:

```latex
\usepackage{btp}
```

or for generating the trainer version of the handout:

```latex
\usepackage[trainermanual]{btp}
```

Commands
========

Here is a list of comands made available by this package. They allow you to define information
about the title, venue, date and authorship of the workshop you intend to deliver.

  * ```\setWorkshopTitle{}```
  * ```\setWorkshopVenue{}```
  * ```\setWorkshopDate{}```
  * ```\setWorkshopAuthor{}```


Paragraph Text Environments
===========================

This style provides several paragraph text environments to make it simpler to get consistent formatting
of text across your handout documents. All without needing to know too much LaTeX! Here is a list of those
provided. 

| Environment Name   | Purpose |
| ------------------ | ------- |
| `information`      | For providing background information to the reader. |
| `steps`            | For providing instructions on the steps the reader is required to take. |
| `note`             | For providing additional information for future reference. |
| `warning`          | For providing a warning which should be read before the reader continues. |
| `questions`        | For posing questions to the reader. |
| `answer`           | For providing the answer to the preceding question. |
| `bonus`            | For providing bonus information, exercises and questions to a quickly advancing reader. |
| `advanced`         | For providing advanced information, exercises and questions to a very quickly advancing reader. |
| `lstlisting`       | For providing code to the reader. |

To use them, simply insert text in between a pair of `\begin{environment-name}` and `\end{environment-name}` statements to have it rendered differently.

Customising the Styling
=======================


License
=======
The contents of this repository are released under the Creative Commons
Attribution 3.0 Unported License. For a summary of what this means,
please see:
http://creativecommons.org/licenses/by/3.0/deed.en_GB
