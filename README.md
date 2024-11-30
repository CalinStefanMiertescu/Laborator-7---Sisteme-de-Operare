Există o aplicație cu mai multe fire. Un fir este fie alb, fie negru, iar firele de execuție trebuie să acceseze o resursă care nu poate fi utilizată simultan de alb și negru, dar poate fi folosită simultan de mai multe fire de același tip.
Protejați împotriva înfometării (starvation).

Observații:
- Poate exista orice număr de fire care solicită acces la resursă, în orice secvență.
- Evitați situațiile în care accesul unui fir este refuzat chiar dacă nu există un alt fir de tip diferit.
- Utilizarea resursei nu este preemptibilă, adică după ce un fir obține acces la resursă, acel fir va folosi resursa atâta timp cât este necesar. Resursa nu poate fi preluată cu forța.
- Utilizarea resursei de către un fir este finită.
- Protecția împotriva înfometării înseamnă că trebuie să garantați că toate firele vor avea acces la resursă, în cele din urmă.

Sarcina:
Trebuie implementat un mecanism care să îndeplinească cerințele atât pentru sistemele Linux, cât și pentru Windows.
