Parts are published in: Computer Methods and Programs in Biomedicine
1997; 191‑200 and the Proceedings of the Nineteenth Annual Symposium on
Computer Applications in Medical Care. 1995; 52--56.

Figure 5--1. Main window of the ABTRANS program to guide a user through
the process of defining a multivariate reference model for acid-base
data. At the left-hand side of the window, the essential five steps to
define a complete model are displayed. Pressing the associated button
activates each step. Results of each step are displayed at the
right-hand side of the window.

Figure 5--2. Patient data editing window (foreground) and laboratory
data editing window (background) of the ABCHART program.

Figure 5--3. Charts and classification window of the ABCHART program. In
the upper left corner the tri-axial chart is displayed with an acid-base
path of a patient. Acid-base measurements are numbered 1 to 25. In the
lower left corner, the time trend of the Mahalanobis distance (here
called 'Abnormality index Dm' for clarity of the user) is shown. Note
that the horizontal line in this plot represents the 30% equal
probability ellipse, displayed as the inner ellipse in the tri-axial
chart. Acid-base measurements falling below the line are inside this
ellipse, while measurements above the line are located outside the
ellipse. In the lower right corner, classifications according the Astrup
and Siggaard-Andersen method and the vector method are given for
acid-base observation number 11.

Figure 5--4. Set-up for automatic data-entry of an ABCHART program
running at an ICU. An arterial blood sample of an ICU patient is sent to
a central clinical chemistry laboratory (Lab) elsewhere in the hospital.
Results of the analysis are sent back to the ICU through the Hospital
Information System (HIS). At the ICU, the incoming serial signal from
the HIS is duplicated by a line-sharing device and sent to both a
printer and a personal computer (PC) installed at the ICU. On the PC, a
running ABCHART program processes the incoming data and performs an
update of its database and windows accordingly.

Table 5--1. Relevant numerical routines used in the programs ABTRANS and
ABCHART.

  -------- -------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------
  name     type           description
  invert   NR-procedure   Calculates the inverse of a matrix. Uses the NR-procedures *ludcmp* and *lubkdsb*.
  moment   NR-procedure   Calculates mean, standard deviation, variance, kurtosis and skewness from an array of input values.
  gammp    NR-function    Incomplete gamma function for the calculation of the theoretical cumulative probability for a specific χ2-value with a given number of degrees of freedom.
  erff     NR-function    Error function for the calculation of a theoretical cumulative probability for a specific Gaussian z-score.
  pearsn   NR-procedure   Returns Pearson's correlation coefficient *r* and corresponding *p*-value for two arrays of input values.
  betai    NR-function    Incomplete beta function for the calculation of a theoretical cumulative probability for a specific F-value with a given number of degrees of freedom.
  jacobi   NR-function    Returns the eigenvectors and eigenvalues of a symmetrical matrix.
  eigsrt   NR-function    Sorts eigenvectors in the eigenvalue matrix after 'jacobi'.
  sKS      VB-function    Calculates the adapted size-adjusted Kolmogorov-Smirnov test-statistic and associated *p*-value for a theoretical and empirical cumulative probability distribution.
  -------- -------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------

**All routines and functions of type NR are from the numerical routines
library *Numerical Recipes in C. The Art of Scientific Computing* (Used
with permission. Copyright © 1987-1992, Numerical Recipes Software)**
**\[2\] and are located in the file NUMREC.DLL. The function of type VB
is written in Visual Basic.**
