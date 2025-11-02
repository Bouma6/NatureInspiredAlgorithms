Použil som základný genetický algoritmus využívajúci crossover a mutácie.
Fitness funkcie ktoré som použil boli : suma jednotiek v jedincovi, počet 0 a 1 na správnom mieste.
Parametre, ktoré som vyskúšal, boli všetky kombinácie:

- mutation = 1, 3, 5
- crossover_prob = 0, 0.5, 1

Ako graf naznačuje, najlepšie výsledky som dosiahol, keď som mutoval iba 1 znak (mutation = 1) a pravdepodobnosť crossoveru bola 100 % (crossover_prob = 1).
Zaujímavé výsledky boli pre mutation 0. Nakolko niekedy algoritmus velmi rýchlo konvergoval do optima ale niekedy konvergoval do určitého bodu odkial sa už bez mutácií nevedel dostať preč a ostal zaseknutý.
Najhoršie výsledky som pozoroval pri vyššej miere mutácie a nižšej pravdepodobnosti crossoveru.

Algoritmus som vždy spúšťal s parametrami:
popsize = 500
generations = 150
individual_size = 100

V každej generácii som mal 500 jedincov.
Algoritmus bežal počas 150 generácií, avšak podľa grafu je vidieť, že vo väčšine prípadov by stačilo približne 60, pretože ďalej už algoritmus výrazne nekonvergoval.
Každý jedinec obsahoval 100 symbolov, ktoré sa v priebehu evolúcie menili.