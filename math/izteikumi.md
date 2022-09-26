## Diskrētā matemātika - Izteikumi

Darbību secība:  $\neg, \land, \lor, \oplus, \rightarrow, \leftrightarrow$

izteikumu loģikas līdzvērtības:

$\neg a = p    \neg p = a$

$A\land p = A     A\lor a = A$

$A \land a = a A \lor p = p$

$\neg\neg A=A$    (divkāršā negācija)

$A\land A = A     A\lor A= A$ (idempotences)

$A \land B = B \land A$ (komutivitāte)

$A \lor B = B \lor A$ (komutivitāte)

$A \land (B\land C) = (A \land B)\land C$ (asociativitāte)

$A \lor (B \lor C) = (A \lor B) \lor C$ (asociativitāte)

$A \land (B \lor C) = (A\land B) \lor (A \land C)$ (distributivitāte)

$A \lor (B \land C) = (A \lor B) \land (A\lor C)$ (distributivitāte)

$\neg (A\land B) = \neg A \lor \neg B$ (dualitāte)

$\neg (A \lor B) = \neg A \land \neg B$ (dualitāte)

$A \land (A \lor B) = A$ (absorbcija)

$A \lor (A \land B) = A$ (absorbcija)

$(A \rightarrow B) \land ( B \rightarrow C) \implies  A \rightarrow C$

| $A, B, C$ | $f(A,B,C)$ | $pDNF$                                   | $pKNF$                                   |
| --------- | ---------- | ---------------------------------------- | ---------------------------------------- |
| $a, a,a$  | $a$        | $-$                                      | $(A \lor B \lor C)\land$                 |
| $a, a, p$ | $p$        | $(\neg A\land \neg B \land C) \lor$      | $-$                                      |
| $a, p, a$ | $p$        | $\lor(\neg A \land B \land \neg C) \lor$ | $-$                                      |
| $a, p, p$ | $a$        | $-$                                      | $\land (A\lor \neg B \lor \neg C) \land$ |
| $p, a, a$ | $a$        | $-$                                      | $\land (\neg A \lor B \lor C) \land$     |
| $p, a, p$ | $p$        | $\lor (A \land \neg B \land C) \lor$     | $-$                                      |
| $p, p, a$ | $a$        | $-$                                      | $ \land (\neg A \lor \neg B \lor C)$     |
| $p, p, p$ | $p$        | $\lor (A \land B \land C)$               | $-$                                      |

$pDNF: f(A,B,C) = (\neg A \land \neg B \land C) \lor (\neg A \land B \land \neg C) \lor (A \land \neg B \land C) \lor (A \land B \land C)$
$pKNF: f(A,B,C) = (A \lor B \lor C) \land (A\lor \neg B \lor \neg C) \land (\neg A \lor B \lor C) \land (\neg A \lor \neg B \lor C)$

$pDNF$ konstruēšana strādā, jo izteiksmes NEKAD neatgriež $p$ pie $A, B, C$ trijnieka, kuram $f(A,B,C)=a$.

$kDNF$ konstruēšana strādā, jo izteiksmes VIENMĒR atgriež $p$ pie $A,B,C$ trijniekiem, kuriem $f(A,B,C)=p$
