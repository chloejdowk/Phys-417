### This project contains two sections:
- Baseline CNN: this contains a combo of four CNN models for four emotional dimensions. Models did binary classification task based on whether the self-reported score go beyound 5 or not. Evan created this baseline model that takes in Raw EEG data for all 32 participants and achieved around 80% training accuracy overall and around 60% validation accuracy.
- RNN + ARCNN: this contains two models made by Chloe: 
    - one is a RNN taking in 10 subjects and doing a regression task over time. The accuracy for RNN model is not very good but generally speaking, valence has the lowest MAE and RMSE loss.
    - Another is an architecture called ARCNN proposed by the paper. It contaisn a channel-wise attention block + CNN + LSTM + self attention + a final classifier. The accuracy for 18 subjects is highest for classifying liking emotion, which reached 94%, while the overall accuracy is not as good as baseline CNN.
    - data was initially processed through baseline removal + spatial/temporal feature extractions
    - DE features on 9 by 9 matrices were inputs for these two models. Several visualizations to visualize the data were made.
