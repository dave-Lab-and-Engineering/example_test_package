# This test fails on purpose

Automated tests can be written in markdown.



## Model:



```load
pendulum.dave
```





## Run

In this case we run statics by specifying some code:

```actions
s.solve_statics()
```



Finally the result is asserted using an assert section

## Tests

Tests are specified using a `assert` section. This section is expected to contain blocks of value=..., expect=... and a description.

```assert
value = s['Cable'].stretch
expected = 23
The expected stretch in the cable is F * L / EA = $10t \cdot 9.81 \cdot 5m / EA = 0.049m$, so 23 is not going to be correct.

```

