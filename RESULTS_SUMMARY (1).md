# Results Summary

## Best Model
- **Model:** KRR-RBF≈@emb {'n_comp': 2048, 'gamma': 0.005, 'alpha': 0.1}  
- **Validation MSE:** ~0.070715  
- **Validation R²:** ~0.884

## Error Distribution
- Residuals (True − Predicted) are tightly centered around 0 with thin tails.  
- Most predictions are very close to actual values; few outliers remain.

## Parity Plot
- Points lie close to the 45° line, indicating strong agreement.  
- Slight underprediction appears at the high end of the target range.

## Comparison with Other Models
- Classical linear models (OLS/Ridge/LASSO/ElasticNet) performed well,  
  but **feature-transfer (NN embeddings + Kernel Ridge RBF)** achieved the best error and variance explained.

## Key Takeaways
1. **Best model:** KRR-RBF≈@emb {'n_comp': 2048, 'gamma': 0.005, 'alpha': 0.1}
2. **Strengths:** Low error, ~88.4% variance explained, well-behaved residuals.
3. **Limitations:** Mild underprediction at extreme values.
4. **Next steps:** Try deeper/wider NN embeddings, gradient boosting (XGBoost/LightGBM), and targeted feature engineering for rare high-target cases.
