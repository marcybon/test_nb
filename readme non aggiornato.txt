# imm_bri
Statistiche partite a briscola 2025

Programma per elaborare i dati delle statistiche delle partite di briscola.

Dati in ingresso: 
- record per ogni partita: 'date W/L chiamante chiamato g1 g2 g3'
Dati sessione recuperabili:
nomi giocatori =5 o più, numero partite = numero di records, partite giocate da ogni giocatore su partite totali di quel giorno e in tutto

Es record:
7gen W Donato Marc Luca Ferro Scalzo
7gen W Donato Bond Luca Ferro Scalzo
7gen L Bond Luca Marc Ferro Scalzo

Calcolo punteggio:
Se W p1(chiamante) +2 p2(chiamato) +1 p3 -1 p4 -1 p5 -1 
Se L p1(chiamante) -2 p2(chiamato) -1 p3 +1 p4 +1 p5 +1 
Se Wv p1(chiamante) +4 p2(chiamato) +2 p3 -2 p4 -2 p5 -2

Calcolo numero partite giocate:
Se nome compare nella riga +1 alle partite giocate da quel giocatore

Percentuale punteggio/punteggio pieno senza contare le vittorie in volata:
Divisione tra punteggio e numero partite*4