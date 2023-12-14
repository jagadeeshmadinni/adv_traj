# adv_traj
Adversarial Robustness Analysis of Trajectron++ model with Apolloscape dataset
This repo is a cloned implementation of https://github.com/zqzqz/AdvTrajectoryPrediction/tree/master with appropriate environment related changes as well as minor config changes to suit computing resource requirements. For original repo, please visit the link mentioned above.

The postProcessing.ipynb notebook contains custom code to calculate the evaluation metrics of the attack optimization from the raw JSON data output and stores them in a CSV called Final_results.

Source links:
1. Formulated test cases and pretrained model for Trajectron++ from https://github.com/zqzqz/AdvTrajectoryPrediction/tree/master
2. Trajectron++ source code to generate input data for preprocessing prior to attack formulation - https://github.com/StanfordASL/Trajectron-plus-plus
3. Apolloscape Dataset - https://github.com/ApolloScapeAuto/dataset-api/tree/master/trajectory_prediction
