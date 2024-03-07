in [[Probability theory|probability theory]] and [[Statistics|statistics]] the Poisson distribution is a [[Discrete probability distribution|discrete probability distribution]] that expresses the probability of a given number of [[Events|events]] occurring in a fixed interval of time if these events occur with a known constant [[Weighted arithmetic mean|mean]] rate and [[Independence|independently]] of the time since the last event.

it can also be used for the number of events in other types of intervals than time, and in dimension greater than $1$ (e.g., number of events in a given area or volume).

under a Poisson distribution with [[Expected value|expectation]] of $\lambda$ events in a given interval., the probability of $k$ events in the same interval is:

$$
\frac{\lambda^{k}e^{-\lambda}}{k!}
$$

# Example

consider a call center which receives, randomly, an average of $\lambda=3$ calls per minute at all times of day. 

if the calls are independent, receiving one does not change the probability of when the next one will arrive. 

under these assumptions the number $k$ of calls received during any minute has a Poisson probability distribution. receiving $k=1$ to $4$ calls has a probability of about $0.77$ while receiving $0$ or at least $5$ calls has a probability of about $0.23$