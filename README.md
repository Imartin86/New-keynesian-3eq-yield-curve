# Modeling the Yield Curve in a New-Keynesian 3EQ Framework

This repository contains a structural macroeconomic model based on the **New-Keynesian Three-Equation (3EQ)** framework. The core objective is to endogenously derive the yield curve by connecting macroeconomic variables (Inflation, Output Gap) with the financial term structure of interest rates.

## 🧠 Theoretical Framework

The model is based on the interaction of the IS equation, the Phillips Curve, and the Monetary Policy (MR) rule. The central innovation is the derivation of a **recursive interest rate rule** that dictates how the Central Bank adjusts rates following a shock.

### Core Recursive Equation
The real interest rate ($r_n$) for any period $n$ is determined by:
$$r_n = r^* + (r_0 - r^*) \left( \frac{1}{1 + \alpha \gamma^2 \beta} \right)^n$$

Where:
- $r^*$: Equilibrium real interest rate.
- $\alpha, \beta, \gamma$: Structural parameters representing the Central Bank's inflation aversion and the slope of the Phillips Curve.



## 📈 Key Simulations (Excel Implementation)

The provided Excel simulations analyze the term structure response to **Permanent Aggregate Demand (AD) Shocks**:

### Case 1: Positive Permanent AD Shock
- **Scenario:** An unexpected increase in autonomous consumption/investment.
- **CB Reaction:** Immediate hike in short-term rates ($r_0$) to curb inflationary pressures.
- **Yield Curve Shape:** **Inversion**. As the Central Bank succeeds in cooling the economy, future expected rates fall towards $r^*$, creating a downward-sloping (inverted) curve.

### Case 2: Negative Permanent AD Shock
- **Scenario:** A sharp contraction in aggregate demand.
- **CB Reaction:** Aggressive monetary easing (lowering $r_t$).
- **Yield Curve Shape:** **Steepening**. The curve becomes positively sloped as markets price in a gradual return to the equilibrium rate as the output gap closes.



## 🛠 Model Assumptions
1. **Expectations Theory:** Long-term yields are the average of expected future short-term rates plus a term premium ($TP$).
2. **Rational Expectations:** Agents perfectly anticipate the Central Bank's systematic response.
3. **No-Shock Horizon:** Post $t=0$, the path of interest rates is deterministic, allowing for the calculation of yields via no-arbitrage conditions.

## 📁 Repository Structure
- `/theory`: Documentation of algebraic derivations and recursive rules (`Macroeconomics_Extra.pdf`).
- `/simulations`: Excel workbooks containing the numerical solvers for the 3EQ dynamics and Yield Curve plotting.

## 🎓 Authors
- Imanol Martín
