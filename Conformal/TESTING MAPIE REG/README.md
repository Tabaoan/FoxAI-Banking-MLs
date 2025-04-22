# MAPIE REG
# Pass
- ### Checkpoint: Core Project
- ### Test 0: Test Calib + prefit like Mapie Clf (wrong)
- ### Test 1: Copy all web tutorial code 
- ### Test 2.0: Copy all web for XGB (comment out STRAT CQR)
- ### Test 2.1: Quick Build 3 model XGB for STRAT CQR (bad result or maybe wrong code)
- ### Test 3.0: Copy all web for LGBM

# Finding best strat for KPI reg
- ### Test 5: Big test for max acceptable width
- ### Test 6: If acceptable 95% width <= 0.1, then find out strat with best coverage of those has width <= 0.1 
- ### >>> Plus is best in all Scenario 
- ### Test 7.0: If acceptavle width <= 0.1, with Plus method, find out quantile that has the best "sure" coverage of those has width <= 0.1
- ### Test 7.1: Clean code to apply more core model like XGB
- ### Test 7.2: Apply XGB >>> Better 

# Final
- ### Test 7.3: Apply best model can find = Catboost >>> Best

# Conclusion:
- ### Plus is best for KPI Scenario Application
    - ### CQR is limited to quantile 4 model
    - ### Naive is can't sendback suspicious prediction
    - ### Plus can fit all model and have highest coverage if width is limited to acceptabl
- ### Core model: The more precise the core model (R2, mae, rmse), the better the coverage of mapie reg (more % "sure" coverage, less % wrong)