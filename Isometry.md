an isometry (or congruent transformation) is a distance-preserving transformation between [[Metric space|metric spaces]], usually assumed to be [[Bijection|bijective]].

from the Greek *isos* (equal) and *metron* (measure). 

if the transformation is from a metric space to itself, it is a kind of [[Geometric transformation|geometric transformation]] known as a [[Motion|motion]].

## Definition

let $X$ and $Y$ be metric spaces with metrics (distances) $d_{x}$ and $d_{y}$. a map $f:X\rightarrow Y$ is called an isometry or distance preserving map if:

$$
\forall a,b\in X \implies d_{x}(a,b)=d_{y}(f(a),f(b))
$$

an isometry is automatically [[Injective functions|injective]] since if two distinct points $a$ and $b$ could be mapped to the same point it would contradict the [[Coincidence axiom|coincidence axiom]] of the metric $d$. ($d(a,b) = 0 \iff a=b$)

a global isometry, isometric isomorphism, or congruence mapping is a bijective isometry; it has a [[Inverse functions|function inverse]].

two metric spaces $X$ and $Y$ are called isometric if there is a bijective isometry from $X$ to $Y$. the [[Sets|set]] of bijective isometries from a metric space to itself forms a [[Group|group]] with a respect to [[Function composition|function composition]], called the [[Isometry group|isometry group]].

there is also path isometry or arcwise isometry which is a map that preserves the [[Arc length|lengths of curves]]; this kind of map is not necessarily an isometry as it doesn't always preserve distance and therefore it is also not necessarily bijective or even injective but is still referred to as an isometry.

# Example Isometries

- [[Reflection|reflection]], [[Translation|translation]], and [[Rotation|rotation]] are global isometries in [[Euclidean space]]. (see also: [[Euclidean group]])
- the map $x\mapsto |x|\in\mathbb{R}$ is a path isometry but not a (general) isometry.