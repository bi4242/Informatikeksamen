Interaktivt, adaptivt system, der tager et spørgsmålssæt som input og giver brugeren spørgsmål vægtet efter, hvad vedkommende svarer mere rigtigt og forkert på. Hvert spørgsmål er associeret med et eller flere tags, som er områder eller emner, de berører. Tags er associeret med en vægt, der stiger, når brugeren svarer forkert, og falder, når brugeren svarer rigtigt. Når brugeren svarer rigtigt på et spørgsmål, fjernes det fra puljen af tilgængelige spørgsmål.

Programmets tilstand består af:
* En vægt associeret med hvert tag.
* En pulje af de spørgsmål, der brugeren ikke har svaret rigtigt på endnu.

Når brugeren svarer rigtigt, ændres vægten af hvert associeret tag med 0,8x.
Når brugeren svarer forkert, ændres vægten af hvert associeret tag med 1,25x.
Et spørgsmål vægtes som produktet af dets tags' vægte.

En flowchart over programmet:

![image](https://github.com/user-attachments/assets/93e67599-463b-4a5f-9ccf-78179feef042)
