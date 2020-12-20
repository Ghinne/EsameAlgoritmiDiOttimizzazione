# EsameAlgoritmiDiOttimizzazione
## Risoluzione di un problema di Agent Scheduling 
### (Traveling Salesman Problem With Time Windows)

### Variabili:
<a href="https://www.codecogs.com/eqnedit.php?latex=\inline&space;\\&space;-\;\boldsymbol{A}:\;&space;Agenti\;assicurazione,&space;\\&space;-\;\boldsymbol{M}:\;Richieste\;di\;Meeting,&space;\\&space;-\;\boldsymbol{g}:&space;Giornata\;lavorativa:\left\{\begin{matrix}&space;Ufficio\;&space;o\;&space;m_1;&space;\\&space;Spostamento;&space;\\&space;Ufficio\;&space;o\;&space;m_2;&space;\\&space;Spostamento;&space;\\&space;\vdots&space;\\&space;Spostamento;&space;\\&space;Ufficio\;&space;o\;&space;m_k;&space;\end{matrix}\right." target="_blank"><img src="https://latex.codecogs.com/gif.latex?\inline&space;\\&space;-\;\boldsymbol{A}:\;&space;Agenti\;assicurazione,&space;\\&space;-\;\boldsymbol{M}:\;Richieste\;di\;Meeting,&space;\\&space;-\;\boldsymbol{g}:&space;Giornata\;lavorativa:\left\{\begin{matrix}&space;Ufficio\;&space;o\;&space;m_1;&space;\\&space;Spostamento;&space;\\&space;Ufficio\;&space;o\;&space;m_2;&space;\\&space;Spostamento;&space;\\&space;\vdots&space;\\&space;Spostamento;&space;\\&space;Ufficio\;&space;o\;&space;m_k;&space;\end{matrix}\right." title="\\ -\;\boldsymbol{A}:\; Agenti\;assicurazione, \\ -\;\boldsymbol{M}:\;Richieste\;di\;Meeting, \\ -\;\boldsymbol{g}: Giornata\;lavorativa:\left\{\begin{matrix} Ufficio\; o\; m_1; \\ Spostamento; \\ Ufficio\; o\; m_2; \\ Spostamento; \\ \vdots \\ Spostamento; \\ Ufficio\; o\; m_k; \end{matrix}\right." /></a>

### Vincoli:
- 30 min per il pranzo tra le 12:00 e le 14:00
- Tempo lavorativo limitato (8 ore);
- Tempo attesa e spostamento limitato;
- Tempo minimo da passare in ufficio (1 ora);

### Funzione obbiettivo:
- Massimizzare attività produttive;
- Prioritizzare i meeting;
- Minimizzare gli spostamenti;
- Favorire grossi blocchi di lavoro uguale (minimizzare i cambiamenti tra lavoro di ufficio e meeting),
