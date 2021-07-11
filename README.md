# Esame Algoritmi Di Ottimizzazione
## Resolution of an Agent Scheduling problem
### (Traveling Salesman Problem With Time Windows)

### Variables:
<a href="https://www.codecogs.com/eqnedit.php?latex=\inline&space;\\&space;-\;\boldsymbol{A}:\;&space;Agents\;,&space;\\&space;-\;\boldsymbol{C}:\;Clients,&space;\\&space;-\;\boldsymbol{wd}:&space;Working&space;\;day:\left\{\begin{matrix}&space;Office\;&space;or\;&space;client_1;&space;\\&space;Travel;&space;\\&space;Office\;&space;or\;&space;client_2;&space;\\&space;Travel;&space;\\&space;\vdots&space;\\&space;Travel;&space;\\&space;Office\;&space;or\;&space;client_k;&space;\end{matrix}\right." target="_blank"><img src="https://latex.codecogs.com/gif.latex?\inline&space;\\&space;-\;\boldsymbol{A}:\;&space;Agents\;,&space;\\&space;-\;\boldsymbol{C}:\;Clients,&space;\\&space;-\;\boldsymbol{wd}:&space;Working&space;\;day:\left\{\begin{matrix}&space;Office\;&space;or\;&space;client_1;&space;\\&space;Travel;&space;\\&space;Office\;&space;or\;&space;client_2;&space;\\&space;Travel;&space;\\&space;\vdots&space;\\&space;Travel;&space;\\&space;Office\;&space;or\;&space;client_k;&space;\end{matrix}\right." title="\\ -\;\boldsymbol{A}:\; Agents\;, \\ -\;\boldsymbol{C}:\;Clients, \\ -\;\boldsymbol{wd}: Working \;day:\left\{\begin{matrix} Office\; or\; client_1; \\ Travel; \\ Office\; or\; client_2; \\ Travel; \\ \vdots \\ Travel; \\ Office\; or\; client_k; \end{matrix}\right." /></a>

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
