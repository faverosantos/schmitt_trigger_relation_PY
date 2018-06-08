# Schmitt trigger calculator

# So, what's the deal?
A Pythonic way of doing what https://www.random-science-tools.com/electronics/inverting-schmitt-trigger-calculator.htm does, except
it lets you set the comparison voltage as a percentage of VREF.

Other examples found on internet:
http://hyperphysics.phy-astr.gsu.edu/hbase/Electronic/schmitt.html
https://www.engineersedge.com/instrumentation/schmitt-trigger.htm
http://www.aaabbb.de/NonInvertingSchmittTrigger/NonInvertingSchmittTrigger_en.php

# How to use?
Choose the reference voltage - VREF, the positive supply voltage (the same as output high voltage) - VDDP,
the negative supply voltage (the same value as the output low voltage) and the porcentage of VREF (PVREF).

For example, setting \
VREF = 2 \
VDDP = 3.3 \
VDDN = 0 \
PVREF = 0.85 
will return R1 = 3, R2 = 1 and R3 = 1.

You can just multiply those values by 10 k and you're set to go.

# Specs
Made with Python 3.6.1