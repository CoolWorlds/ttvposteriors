# ttvposteriors
Joint posterior samples from Kipping, D., 2020, "An Independent Analysis of the Six Recently Claimed Exomoons", The Astropysical Journal Letters, Accepted.

Files beginning with T_ correspond to posterior sample files for model T, which accounts for transit timing variations. In some cases, a KOI has two files for model T, denoted by the suffix "\_1.dat" and "\_2.dat" which correspond to the two segments used (see the paper for details). For T files, the first 7 columns correspond to the global shape parameters of the transit, which are...\\

1] R_p/R_*\\
2] rho_* [km/m3]\\
3] b
4] P [days]
5] tau_0 [BJDutc - 2,400,000]
6] q_1 (limb darkening coefficient, see 2013MNRAS.435.2152K)
7] q_2 (limb darkening coefficient, see 2013MNRAS.435.2152K)

Note that P and tau0 are merely reference values in model T and are not regressed. The subsequent columns (>7) correspond to each epoch's time of transit minimum (tau_i)

Files beginning with M_ correspond to posterior sample files for model M, which regresses the LUNA photodynamical moon model (2011MNRAS.416..689K) to the data. The first 7 columns are the same as model T, but the next 7 are:

8] P_s
9] a_s/R_p
10] phi_s (phase)
11] cos(i_s)
12] Omega_s
13] M_s/M_p
14] Rs/R_p

Finally, the files beginning with AVG_ are the method marginalized light curves for each KOI (time, intensity, error)
