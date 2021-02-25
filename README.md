# OptionPricing
Black&amp;Scholes Closed formula | Monte-Carlo for BS and Exotic Options | EDS &amp; Heston Model
## Modèle de Black&Scholes

### Formulation
On considère un \textbf{actif risqué} de prix $S$, stochastique, de dynamique :
\begin{myequation}
\mathrm{d}S_t = \mu S_t \mathrm{dt} + \sigma S_t \mathrm{d}B_t
\end{myequation}

Avec $\mu$ représentant le drift (tendance), et $\sigma > 0$ la volatilité.

En passant au log et en appliquant Itô sur $Y_t = log(S_t)$, nous obtenons la solution :
\begin{myequation*}
S_t = S_{0}e^{\left(\mu - \frac{\sigma^{2}}{2}\right)t + \sigma B_t}
\end{myequation*}

Nous admettons que $(S_t)_{t \in [0,T]}$ est un processus continu, dont les composantes suivent une loi log-normale. 
Les rendements sont donc, sous nos hypothèses, stationnaires et indépendants.

Également, nous considérons un \textbf{actif sans risque} de prix $D$ déterministe, croissant au taux sans risque $r > 0$ tel que :
\begin{myequation*}
\mathrm{d}D_t = rD_t
\end{myequation*}

Avec $D_0 = 1$, nous avons donc en résolvant l'équation :
\begin{myequation*}
D_t = e^{rt}
\end{myequation*}
Généralement, le taux $r$ peut être vu comme le taux d'une oligation zéro coupon.

Ce taux sans risque permet d'introduire le principe d'\textbf{actualisation (discount)}, représentant la "valeur-temps" de l'argent, tel que : 
\begin{myequation*}
\overset{\sim}{S_t} = e^{-rt}S_t
\end{myequation*}

Nous avons ainsi :
\begin{myequation}
\mathrm{d}\overset{\sim}{S_t} = (\mu-r) \overset{\sim}{S_t} \mathrm{dt} + \sigma \overset{\sim}{S_t} \mathrm{d}B_t 
\end{myequation}

