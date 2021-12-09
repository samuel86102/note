## Data Mining Midterm Exam Notes by Samuel

#### GINI index

$GINI(t)=1- \sum_{j=1}^{n_C} p(j|t)^2$

$GINI_{split}= \sum_{i=1}^{k} \frac{n_i}{n}GINI(i)$

$Gain = P - M$

---

#### Confusion matrix
 _ | _ | Predicted | Class
---|---|---     |---
 _ | _ | class=1| class=0
Actual|class=1|TruePositive|FalseNegative
Class  |class=0|FalsePositive|TrueNegative

- Accuracy = $\frac{TP+TN}{TP+TN+FP+FN}$

- Precisionin ($p$) = $\frac{TP}{TP+FP}$

- Recall ($r$) = $\frac{TP}{TP+FN}$

- F-measure = $\frac{2rp}{r+p}$

---

#### FOIL Information Gain
$\text{FOIL's information gain}=p_1 \times (log_2 \frac{p_1}{p_1+n_1}-log_2 \frac{p_0}{P_0+n_0})$

- larger information gain $\rightarrow$ more accurate
- when $gain\le0$ $\rightarrow$ no improvement

---
#### Data Normalization
$$
x_{i}^{'} = \frac{x_i-\text{min}_i\{x_i\}}{\text{max}_i\{x_i\} - \text{min}_i\{x_i\}}
$$

---
#### Bayes Theorem
$$
P(Y|X) = \frac{P(X|Y)P(Y)}{P(X)}
$$
---
#### Cosine Similarity
> the $\cos{\theta}$ of two vectors
$$
\text{similarity(A,B)} = \frac{A \cdot B}{||A|| \times ||B||} \in \bm{[0,1]}
$$

---

#### Similarity Between Binary Vectors
- $\text{SMC} = \frac{(f_{11}+f_{00})}{(f_{01}+f_{10}+f_{11}+f_{00})}$

- $\text{Jaccard} = \frac{(f_{11})}{(f_{01}+f_{10}+f_{11})}$
  - Take off all $f_{00}$, more suitable for asymmetric(0 or 1 dominates)

---
#### Minkowski Distance
$$
d(p,q)=(\sum_{k=1}^n|x_k-y_k|^{r})^{\frac{1}{r}}
\\~\\
\text{r=1, Hamming distance, L1 norm}
\\~\\
\text{r=2, Euclidean distance}
\\~\\
\text{r}\rightarrow \infin \text{, supremum}
$$
---







