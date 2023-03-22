# EKI-Subsampling
Subsampling algorithm for ensemble Kalman inversion

The file consists of 3 main files: "Heat_equation_EKI_para.m", "Heat_equation_Eki_para_vi.m" and "reference_data_df_kl_para.m". Those files contain the algorithms for the ensemble Kalman inversion as well as our subsampling alogrithms. To run this files first one has to run "gen_heat_eki_params.m" (respectively "gen_heat_EKI_params_vi.m" and "gen_nonlin_darcy_params.m"). This files initialize the system with parameters, if you want to try different parameters you should only change the values in these files.

Furthermore, the results are always saved in sepereate files ("NumericsLin" and "NumericsNonLin/Coefficients") and are called later again in the evaluation. Therefore you need to generate these respective folders before running the algorithm.

One run for the Heat equation example usually runs ~90 minutes, for the 2D-Darcy flow ~5 hours. We therefore recommend parallel computing (which is also the implemented method).
