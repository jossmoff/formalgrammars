## Commands

### \pr
  - **Description**: Creates a production rule to be put into the grammar.
  - **Usage**: `\pr{var}{str_of_vard_and_terms}`
  - **Example**: 
  ```latex 
  \pr{S}{aSb}
  ```
### \gor
 - **Description**: Creates an or in production rule WITHOUT trailing white space.
 - **Usage**: `\gor`
 - **Example**:
 ```latex
 \pr{NN}{steel \gor alloy \gor carbon \gor base \gor metal}
 ```
### \gors
 - **Description**: Creates an or in production rule with a single trailing white space.
 - **Usage**: `\gors`
 - **Example**: 
 ```latex
 \pr{NN}{steel \gors alloy \gors carbon \gors base \gors metal}
 ```
 
 ### \yields
 - **Description**: Alias for the yields symbol in Sipsers CFG definition..
 - **Usage**: `\yields`
 - **Example**:
 ```latex
 uAv \yields uvw
 ```
 
 ### \derives
 - **Description**: Alias for the derive symbol in Sipsers CFG definition.
 - **Usage**: `\derives`
 - **Example**: 
 ```latex
 u \derives v
 ```
## Enviroments 

### grammar
 - **Description**: Creates a production rule to be put into the grammar.
 - **Usage**: `\begin{grammar}{prod_rules}
               \end{grammar}`
 - **Example**: 
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
