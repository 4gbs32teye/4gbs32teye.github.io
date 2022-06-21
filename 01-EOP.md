
# The Elements of Probability {-}

## Terminology and Definitions {-}

**Event** : A set, class, or group of possible uncertain outcomes.

  - **Compound Event** : An event that can be decomposed into sub-events.
  - **Elementary Event** : An event that cannot be further decomposed.


**Event Space** : Also known as the **Sample Space**, is the set of all possible
elementary events. The sample represents the universe of all possible events. It
can be thought of as the largest possible compound event.

**Mutually Exclusive and Collectively Exhaustive (MECE)** : A sample in which no
more than one event can occur at a time (mutually exclusive) and that at least
one of the events will occur (collectively exhaustive).

**The Axioms of Probability**

  1. The probability of any event is non-negative.
  1. The probability of the sample space $S$ is $Pr\{S\}=1$. In other words, the
  sum of probabilities for all possible outcomes is 1.
  1. The probability that one or the other of two mutually exclusive events
     occurs is the sum of their probabilities.

**Law of Large Numbers** : The _frequentist interpretation_ that the ratio of the
number of occurances of the event $\{E\}$ to the total number of opportunities for
$\{E\}$ in a sample will approach the probability of $\{E\}$, written as $Pr\{E\}$.

**Complement** : The (usually compound) event where $\{E\}$ does not occur. Its
probability can be expressed as, $$Pr\{E^C\} = 1 - Pr\{E\}$$

**Joint Probability** : The probability that more than one event will occur, expressed
as their intersection ($\cap$). For the simple case where there are only two events, 
this is represented by the region where two circles overlap on a Venn diagram.
$$Pr\{E_1 \cap E_2\} = Pr\{E_1 \ \ and \ \ E_2\}$$

**Additive Law of Probability** : The probability that at least one event will occur
expressed as their union ($\cup$). For the simple case where there are only two
events, this is represented by the region encompassed by $E_1$ and $E_2$ on a Venn
diagram, subtracting where they intersect to avoid double-counting.
$$Pr\{E_1 \cup E_2\} = Pr\{E_1\} + Pr\{E_2\} - Pr\{E_1 \cap E_2\}$$

**DeMorgan's Laws**

  - The complement of a union of two events equals the intersection of the
  complements of the two individual events.

  $$Pr\{(A \cup B)^C\} = Pr\{A^C \cap B^C\}$$
  
  - The complement of the intersection of two events equals the union of the
  complements of the two individual events.

  $$Pr\{(A \cap B)^C\} = Pr\{A^C \cup B^C\}$$

**Conditional Probability** : Expressed as $Pr\{E_1 | E_2\}$ for the simple case
of two events. It can be read as "the probability of $E_1$ given $E_2$". Here, $E_2$
is the _conditioning event_, which essentially defines the sample space. In other
words, the "given-ness" of $E_2$ means that in this case only events where $E_2$
occurred are considered in the calculation. The probability of $E_1$ is the ratio
of the intersection of $E_1$ with $E_2$, and $E_2$:
$$Pr\{E_1 | E_2\} = \frac{Pr\{E_1 \cap E_2\}}{Pr\{E_2\}}$$

**Multiplicative Law of Probability** : A rearrangement of the definition of
conditional probability. Namely,

$$Pr\{E_1 \cap E_2\} = Pr\{E_1 | E_2\} * Pr\{E_2\}$$

Or, in a more familiar form, for independent events,

$$Pr\{E_1 \cap E_2\} = Pr\{E_1\} * Pr\{E_2\}$$

**The Law of Total Probability** : Consider a set of $N$ mutually exclusive collectively
exhaustive (MECE) events, $\{E_i\}$. If there is another event $\{A\}$ also defined within
this sample space, its probability can be computed by summing the joint probabilities.

$$Pr\{A\} = \displaystyle\sum_{i=1}^{N} Pr\{A \cap E_i\} = \displaystyle\sum_{i=1}^{N} Pr\{A | E_i\} * Pr\{E_i\}$$

