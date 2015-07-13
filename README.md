We suggest that you do not use this repository directly unless you know what you are doing. Instead, you should 
probably head over to the [btp-workshop-template](https://github.com/BPA-CSIRO-Workshops/btp-workshop-template)
repository and follow one of the
[workflows](https://github.com/BPA-CSIRO-Workshops/btp-workshop-template#general-workflows) documented there.

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

Paragraph Text Environments
===========================

| Environment Name | Purpose |
| ---------------- | ----- |
| information      | For providing background information to the reader. |
| steps            | For providing instructions on the steps the reader is required to take. |
| note             | For providing additional information for future reference. |
| warning          | For providing a warning which should be read before the reader continues. |
| questions        | For posing questions to the reader. |
| answer           | For providing the answer to the preceding question. |
| bonus            | For providing bonus information, exercises and questions to a quickly advancing reader. |
| advanced         | For providing advanced information, exercises and questions to a very quickly advancing reader. |
| lstlisting       | For providing code to the reader. |
