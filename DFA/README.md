### a) Definition der Sprache $L_1$

Sei  
```math
L_1 := \{ w \mid w \in \{a, b\}^* \text{ und } w \text{ enthält } aa \text{ oder } bb \text{ als Infix} \}
```

**Bemerkung:** Ein Wort $v$ ist ein *Infix* von $w$, falls es Wörter $u, x \in \{a, b\}^*$ gibt, sodass  
$w = u v x$ gilt

---

### b) Definition der Sprache $L_2$

Sei
```math
L_2 := \overline{L_1} = \{a, b\}^* \setminus L_1
```
Das heißt, $L_2$ enthält alle Wörter über dem Alphabet $\{a, b\}$, die **nicht** das Teilwort (Infix) $aa$ oder $bb$ enthalten.

---
### c) Operationen: DFA Vereinigung, Schnitt, Multipilkation

Konstruktion von Automaten für 
```math
L(M_1) \cap L(M_2), L(M_1) \cup L(M_2)\text{ und }L(M_1)L(M_2)
```
Gegeben sind die deterministischen endlichen Automaten:
```math
M_1 = (\{z_0, z_1, z_2\}, \{a, b\}, \delta_1, z_0, \{z_1\})
```
mit:

$\delta_1(z_0, a) = z_0$, $\delta_1(z_0, b) = z_1$,
$\delta_1(z_1, a) = z_2$, $\delta_1(z_1, b) = z_2$,
$\delta_1(z_2, a) = z_2$, $\delta_1(z_2, b) = z_2$.

```math
M_2 = (\{s_0, s_1\}, \{a, b\}, \delta_2, s_0, \{s_1\})
```
mit:

$\delta_2(s_0, a) = s_1$, $\delta_2(s_0, b) = s_0$
$\delta_2(s_1, a) = s_0$, $\delta_2(s_1, b) = s_1$



Konstruieren Sie die folgenden endlichen Automaten:
1. $M_\cap$, der die Sprache $L(M_1) \cap L(M_2)$ akzeptiert
2. $M_\cup$, der die Sprache $L(M_1) \cup L(M_2)$ akzeptiert
3. $M_\circ$, der die Sprache $L(M_1)L(M_2)$ akzeptiert




```math
```
