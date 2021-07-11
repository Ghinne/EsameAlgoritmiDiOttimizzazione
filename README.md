# Esame Algoritmi Di Ottimizzazione
## Resolution of an Agent Scheduling problem
### (Traveling Salesman Problem With Time Windows)

### Variables:
<a href="https://www.codecogs.com/eqnedit.php?latex=\inline&space;\\&space;-\;\boldsymbol{A}:\;&space;Agenti\;assicurazione,&space;\\&space;-\;\boldsymbol{M}:\;Richieste\;di\;Meeting,&space;\\&space;-\;\boldsymbol{g}:&space;Giornata\;lavorativa:\left\{\begin{matrix}&space;Ufficio\;&space;o\;&space;m_1;&space;\\&space;Spostamento;&space;\\&space;Ufficio\;&space;o\;&space;m_2;&space;\\&space;Spostamento;&space;\\&space;\vdots&space;\\&space;Spostamento;&space;\\&space;Ufficio\;&space;o\;&space;m_k;&space;\end{matrix}\right." target="_blank"><img src="https://latex.codecogs.com/gif.latex?\inline&space;\\&space;-\;\boldsymbol{A}:\;&space;Agenti\;assicurazione,&space;\\&space;-\;\boldsymbol{M}:\;Richieste\;di\;Meeting,&space;\\&space;-\;\boldsymbol{g}:&space;Giornata\;lavorativa:\left\{\begin{matrix}&space;Ufficio\;&space;o\;&space;m_1;&space;\\&space;Spostamento;&space;\\&space;Ufficio\;&space;o\;&space;m_2;&space;\\&space;Spostamento;&space;\\&space;\vdots&space;\\&space;Spostamento;&space;\\&space;Ufficio\;&space;o\;&space;m_k;&space;\end{matrix}\right." title="\\ -\;\boldsymbol{A}:\; Agenti\;assicurazione, \\ -\;\boldsymbol{M}:\;Richieste\;di\;Meeting, \\ -\;\boldsymbol{g}: Giornata\;lavorativa:\left\{\begin{matrix} Ufficio\; o\; m_1; \\ Spostamento; \\ Ufficio\; o\; m_2; \\ Spostamento; \\ \vdots \\ Spostamento; \\ Ufficio\; o\; m_k; \end{matrix}\right." /></a>

### Constraints:
- 30 min lunch between 12:00 and 14:00;
- Limited working time (8 hours);
- Limited waiting and traveling time;
- Minimum time to spend in office (1 hour);

### Objective function:
- Maximize productive activities;
- Priorityze meetings;
- Minimize travels;

## Models:
### [Integer Linear Programming](https://github.com/Ghinne/EsameAlgoritmiDiOttimizzazione/blob/main/ESAMEILP.pdf)
### [Dynamic Programming]()
