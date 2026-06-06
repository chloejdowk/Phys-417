### This repository is created for PHYS417 SPR 26.
There are 7 folders for 7 different labs, including following
- [Lab 1 Report: Data Preparation Techniques for Machine Learning](<https://github.com/chloejdowk/Phys-417/tree/a66170e0f84c8249236b107d0663ef23e745ea29/Lab_1>)
- [Lab 2 Report: Iris Classification with Regression](<https://github.com/chloejdowk/Phys-417/tree/a66170e0f84c8249236b107d0663ef23e745ea29/Lab_2>)
- [Lab 3 Report: MNIST Classification with FCN](<https://github.com/chloejdowk/Phys-417/tree/a66170e0f84c8249236b107d0663ef23e745ea29/Lab_3>)
- [Lab 4 Report: Surpass Human Performance in Fashion MNIST Classificaion with CNN + FCN](<https://github.com/chloejdowk/Phys-417/tree/a66170e0f84c8249236b107d0663ef23e745ea29/Lab%204>)
- [Lab 5 Report: Create Arthur Conan Doyle AI with RNN](<https://github.com/chloejdowk/Phys-417/tree/a66170e0f84c8249236b107d0663ef23e745ea29/Lab_5>)
- [Lab 6 Report: German-to-English Translation with Attention-Mechanism Transformer Model](<https://github.com/chloejdowk/Phys-417/tree/b32010ea86cc50a2d36eb6055826ea9aaca3357f/Lab%206>)
- [Lab 7 Report: Agentic Signal versus Background Classification for Exotic Higgs Decays](<https://github.com/chloejdowk/Phys-417/tree/b32010ea86cc50a2d36eb6055826ea9aaca3357f/Lab%207>)
- [**Final Project: EEG Emotion Classification**](<https://github.com/chloejdowk/Phys-417/tree/b32010ea86cc50a2d36eb6055826ea9aaca3357f/Final_project>)

### Final Project
For this class, our group tested three different models on DEAP dataset for EEG classification on 4 emotional dimensions: Valence, Arousal, Dominance, and Liking.
### This project contains two sections:
- Baseline CNN: this contains a combo of four CNN models for four emotional dimensions. Models did binary classification task based on whether the self-reported score go beyound 5 or not. Evan created this baseline model that takes in Raw EEG data for all 32 participants and achieved around 80% training accuracy overall and around 60% validation accuracy.
- RNN + ARCNN: this contains two models made by Chloe: 
    - one is a RNN taking in 10 subjects and doing a regression task over time. The accuracy for RNN model is not very good but generally speaking, valence has the lowest MAE and RMSE loss.
    - Another is an architecture called ARCNN proposed by the paper. It contaisn a channel-wise attention block + CNN + LSTM + self attention + a final classifier. The accuracy for 18 subjects is highest for classifying liking emotion, which reached 94%, while the overall accuracy is not as good as baseline CNN.
    - data was initially processed through baseline removal + spatial/temporal feature extractions
    - DE features on 9 by 9 matrices were inputs for these two models. Several visualizations to visualize the data were made.

** Eventually, this work was presented at the class symposium as a [poster presentation](<https://github.com/chloejdowk/Phys-417/blob/b32010ea86cc50a2d36eb6055826ea9aaca3357f/Final_project/Emotional%20EEG%20Poster.pdf>)
