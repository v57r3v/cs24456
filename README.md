java c
Problem Set 1
Due: Friday, February 7, 5:00 p.m. Eastern Time
Submission Instructions: Upload a Single PDF File to Canvas, under “Assignments”
Applied Econ 440.602: Macroeconomic Theory
Spring, 2025
1. Growth Rates. In this question, you’re asked to consider some variable — call it xt — that’s changing over time. The subscript. t refers to the time at which the variable is observed, so the sequence of numbers x1, x2, x3, . . . refers to values of the variable in time periods 1, 2, 3, . . .. For example, if xt stands for GDP, and if GDP is measured on a yearly basis, then x1 would stand for GDP in year 1, x2 would stand for GDP in year 2, and so on. GDP is a concrete example of a variable that’s changing over time, but the ideas here apply to any variable that’s changing over time.
Let’s introduce the notation ∆xt to refer to the change in xt between periods t − 1 and t:
∆xt ≡ xt − xt−1.                       (1)
Notice the “≡” in the above expression; this symbol means that ∆xt is defined as xt − xt−1. Again, for example, suppose that xt stands for GDP in year t; then, ∆xt is the change in GDP between year t − 1 and year t. If we write ∆x2, then it means the change in GDP between year 1 and year 2:
∆x2 = x2 − x1.                               (2)
The difference in a variable between period t − 1 and period t should not be confused with the growth rate of a variable between period t−1 and period t. Let’s introduce the notation %∆xt to refer to the growth rate of xt between period t − 1 and period t:
%∆xt ≡ xt−1/xt − xt−1.                                (3)




As before, the “≡” means that %∆xt is defined as   xt−1/xt − xt−1.   Whereas ∆xt is the change in xt from one time period to the next, %∆xt is the percent change or the growth rate. Notice that saying %∆xt = g is equivalent to saying:






xt = (1 + g) × xt−1.                                        (4)
Equation (4) comes from replacing %∆xt with g in equation (3) and rearranging terms. As a point of caution, %∆xt needs to be multiplied by 100 to be converted to a proper percentage: Saying that “xt grew by 5%” is equivalent to saying that %∆xt = .05. Calculations involving growth rates arise frequently in macroeconomics. Economic growth refers to the growth rate of real output; inflation refers to the growth rate of prices; a rate of return refers to the growth rate of the value of an asset.
(a) Suppose that xt = yt + zt. Show that the growth rate of xt is a weighted average of the growth rates of yt and zt:
%∆xt = xt−1/yt−1 × %∆yt + xt−1/zt−1 × %∆zt.                                    (5)






In general, when I ask you to show something, I mean that you should justify the given statement as being correct. In this case, I’m asking you to verify that equation (5) is correct, given that xt = yt + zt, and given the definitions of %∆xt, %∆yt, and %∆zt. It’s acceptable for you to undertake any sequence of steps that makes the left-hand side of equation (5) equal to the right-hand side. You just have to make it clear what steps you’re undertaking, and in what order.




(b) Suppose that xt = yt × zt. Show that:
(1 + %∆xt) = (1 + %∆yt) × (1 + %∆zt).                                (6)
(c) In many applications, percent changes are practically small at short horizons. For example, quarterly real GDP growth and quarterly inflation in the U.S. have historically been in the single digits. Suppose that %∆yt ×%∆zt ≈ 0. (If yt and zt each grow by one percent, for example, then %∆yt = %∆zt = .01, so %∆yt × %∆zt = .0001, which is one percent of one percent.) Show that, if xt = yt × zt, then the growth rate in xt is approximately the sum of the growth rates of yt and zt:
%∆xt ≈ %∆yt + %∆zt.                                           (7)
To justify equation (7), you can take equation (6) as given. If xt = yt ÷ zt, then how would you approximate %∆xt in terms of %∆yt and %∆zt?
(d) Let’s test the accuracy of the approximation you just derived in question 1c, while also getting acquainted with some actual data on the U.S. economy. A useful source of economic data is FRED, which is maintained by the Federal Reserve Bank of St. Louis: https://fred.stlouisfed.org/. Download quarterly seasonally adjusted data on nominal GDP and real GDP. (In FRED, the variable code for nominal G代 写Econ 440.602: Macroeconomic Theory Problem Set 1 Spring, 2025Matlab
代做程序编程语言DP is GDP, and the code for real GDP is GDPC1.) Recall that:
Nominal GDP = Real GDP × Price Level.                                           (8)
For each date t for which data is available, compute a price level series pt by taking the ratio of nominal to real GDP. (This measure of the price level is called the GDP deflator.) The inflation rate is defined as the growth rate of the price level in the economy. For each date t, compute the (exact) inflation rate as %∆pt, and plot your results over time. Now, use the approximation from question 1c to calculate the (approximate) inflation rate as the growth rate of nominal GDP minus the growth rate of real GDP. Plot the difference between the exact inflation rate and the approximate inflation rate. Is the approximation a good one?
2. Logs and Growth Rates. Recall the definition of the natural logarithm: We say that log (x) = y if x = ey, where e = 2.718 . . . is a known constant. Taking the log of a variable can provide a useful data transformation. For the purposes of treating data, it might help just to think of the log function as a particular function with some appealing properties, which we will explore in the questions below.
(a) Recall the following property of exponents:
ab × ac = ab+c,                                                   (9)
where a is any positive number. Given the above, show that:
log (x × y) = log (x) + log (y)                                (10)
log (x ÷ y) = log (x) − log (y).                               (11)
(b) Consider a sequence of numbers: x0, x1, x2, . . .. Define yt ≡ log (xt). If %∆xt is equal to gt, then what is ∆yt?
(c) If ϵ is a small number, then one can use the first-order Taylor-series approximation:
log (1 + ϵ) ≈ ϵ.                                            (12)
Again, growth rates of economic variables are often small over short horizons. Argue that, if yt = log (xt) and %∆xt is close to zero, then:
∆yt ≈ %∆xt.                                           (13)
Hint: Use your answer from question 2b and apply the approximation for log (1 + ϵ).




(d) As before, we can look at some real data to see how well this approximation works in practice. Using the data on the GDP deflator from question 1d, let pt denote the price level. For each date t for which data is available, calculate exact the exact inflation rate as %∆pt, and calculate the approximate inflation rate ∆ log (pt). Plot the difference between the exact inflation series and the approximate inflation series. Is the approximation a good one? (Hint: If you’re doing this in Microsoft Excel, then use the function LN to compute natural logs.)
3. Real vs. Nominal Interest Rates. The U.S. Treasury sells a type of bond called a Treasury Inflation-Protected Security (TIPS). The amount that these bonds pay out is indexed to inflation, so if the price of goods and services goes up, then you receive more cash when the bond matures. Precisely, if you buy a TIPS at time t with a face value of F and a maturity of n, then the Treasury promises to give you pt/pt+n F dollars in period t + n. Here, pt is the Consumer Price Index (CPI), which measures the cost of a basket of commonly consumed goods.
(a) Write the bond’s payout pt/pt+n F in terms of the path of inflation (πt+1, πt+2, . . . , πt+n), where πt ≡ pt−1/pt−pt−1. (Your answer should also contain F, but not any pt terms.)






(b) Is the yield to maturity on TIPS a real interest rate or a nominal interest rate? Why?
(c) Go to FRED (https://fred.stlouisfed.org/) and download data on the yields for 5-year TIPS and 5-year standard treasury bonds. The codes for these variables in FRED are DFII5 and DGS5, respectively. Use the monthly versions of these variables, which you can get by clicking on “Edit Graph” and using the drop-down menu for “Modify Frequency” to select “Monthly.”
i. Make two graphs. On the first, plot the two series for yields on the same set of axes. On the second graph, plot the difference between the yield on the standard bond and the yield on the inflation-protected bond. The graphs should include all dates for which both series are available (2003 to present).
ii. Do the two yield series tend to move together? How do you interpret the difference between the two yields?









         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
