# LaTeX style for Formal Grammars

LaTeX style for Formal Grammars and operations

In order to load the package, use the following code:

```latex
\usepackage{formalgrammars}
```

Once you have done this you can now create your grammar by creating a grammar enviroment and passing it a list of production rules.

```latex 
\begin{grammar}{
    \pr{S}{NP VP}
    \pr{VP}{VBZ NP}
    \pr{PP}{IN NP}
    \pr{NP}{NN \gors DT NN \gors NP PP}
    \pr{NN}{steel \gors alloy \gors carbon \gors base \gors metal}
    \pr{VBZ}{is \gors contains}
    \pr{DT}{an \gors the}
    \pr{IN}{of}}
\end{grammar}
```

Will output as the following:

See the documenation here : [Coming Soon]()
