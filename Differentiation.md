is the process of finding the [[Derivative|derivative]] of a [[Function|function]]. in principle, the derivative can be computed from the definition by considering the difference quotient and computing its limit.

imagine you are on a road trip. the speedometer in your car shows your speed at any given moment, which how fast you're covering distance over time. speed in this example is the derivative of your position with respect to time.

now imagine you're looking at your trip's start and end points. you know the total distance and total time taken. 

you can calculate your average speed over the whole trip by taking the ratio of these two values. this is similar to the difference quotient. its like an average rate of change of the function over a certain interval. 

more specifically we are looking at instantaneous time so the interval becomes an [[Infinitesimal|infinitesimal]].

mathematically, for a function $f(x)$ the difference quotient is 

$$
\frac{f(x+h)-f(x)}{h}
$$

where you are measuring the change in the function's output ($f(x+h)-f(x)$) for a small change in input ($h$).

this small change in input will quickly cause the output to approach zero and that's where [[Limit|limits]] get involved.

finding the limit of the difference quotient as $h$ approaches $0$ gives you the function's rate of change (or [[Slope|slope]]) at that exact moment (instantaneous). 

$$
\lim_{h\rightarrow 0}\frac{f(x+h)-f(x)}{h}
$$

(see also: [[Differentiation rules|differentiation rules]])