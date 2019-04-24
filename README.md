#!/usr/bin/env python3
# -*- coding:utf-8 -*-

import math
import sys

try:
    salary = int(sys.argv[1])
    nashuie = salary - 5000
    if nashuie < 0:
        print("salary is {} <= 5000".format(salary))
    elif nashuie <= 3000:
        geshui = nashuie * 0.03
        print(format(geshui,".2f"))
    elif nashuie <= 12000:
        geshui = nashuie * 0.1 - 210
        print(format(geshui,".2f"))
    elif nashuie <= 25000:
        geshui = nashuie * 0.2 - 1410
        print(format(geshui,".2f"))
    elif nashuie <= 35000:
        geshui = nashuie * 0.25 - 2660
        print(format(geshui,".2f"))
    elif nashuie <= 55000:
        geshui = nashuie * 0.3 - 4410
        print(format(geshui,".2f"))
    elif nashuie <= 80000:
        geshui = nashuie * 0.35 - 7160
        print(format(geshui,".2f"))
    else:
        geshui = nashuie * 0.45 - 15160
        print(format(geshui,".2f"))
except ValueError:
     print("Parameter Error")

