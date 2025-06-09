### a) Definition der Sprache $L_1$

Sei  
$$
L_1 := \{ w \mid w \in \{a, b\}^* \text{ und } w \text{ enthält } aa \text{ oder } bb \text{ als Infix} \}
$$

**Bemerkung:** Ein Wort $v$ ist ein *Infix* von $w$, falls es Wörter $u, x \in \{a, b\}^*$ gibt, sodass  
$$
w = u v x
$$

---

### b) Definition der Sprache $L_2$

Sei  
$$
L_2 := \overline{L_1} = \{a, b\}^* \setminus L_1
$$

Das heißt, $L_2$ enthält alle Wörter über dem Alphabet $ \{a, b\} $, die **nicht** das Teilwort (Infix) $ aa $ oder $ bb $ enthalten.