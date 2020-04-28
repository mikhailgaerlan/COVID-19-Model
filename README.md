**COVID-19 Model**

An SIR model with a time-dependent, exponentially-decaying reproduction number.

This model is based off data from JHU CSSE at https://github.com/CSSEGISandData/COVID-19.

My model assumes full immunity after infection and continued shelter-in-place orders to drive down the reproduction number.

I used a finite difference model to fit the parameters to existing data, then used an IVP ODE solver to extrapolate the model.

Using the parameter covariance matrix, I estimated the 95% confidence interval through a Monte Carlo simulation drawing from a multivariate normal distribution.

The x-axis represents current day of the year. For reference April 25 is the 116th day of 2020.

![US Projection](usprojection.png)

Assuming these conditions, peak cases will occur around May 15 with an approximated ~115K deaths by then.

<script type="text/javascript" src="https://latex.codecogs.com/latexit.js"></script>
<script type="text/javascript">
LatexIT.add('p',true);
</script>LatexIT.add('p',true);
<p>$t^2$</p>
