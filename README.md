# neuro
Computational neuroscience demos

So far, this repository only contains a Python implementation of the Hodgkin-Huxley model of
action potential initiation.

I've used separate functions for the voltage-dependent target (equilibrium) levels of Na
activation (m), Na inactivation (h), and K activation (n), even though the functional
forms are, as things stand, the same; ditto for the associated voltage-dependent timescales.
This is to allow for flexibility. For example, users can easily change the functional form
of target Na activation without changing the other functions.

Numerical integration is handled by scipy's initial value problem solver (solve_ivp).
