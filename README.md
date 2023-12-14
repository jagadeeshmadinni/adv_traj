# adv_traj
Adversarial Robustness Analysis of Trajectron++ model with Apolloscape dataset
This repo is a cloned implementation of https://github.com/zqzqz/AdvTrajectoryPrediction/tree/master with appropriate environment related changes as well as minor config changes to suit computing resource requirements. For original repo, please visit the link mentioned above.

The postProcessing.ipynb notebook contains custom code to calculate the evaluation metrics of the attack optimization from the raw JSON data output and stores them in a CSV called Final_results.

To replicate the results, clone the AdvTrajectoryPrediction and follow the instructions on the repo homepage to download the test cases and pretrained model. Run the following command after navigating to the **test** directory:
python test.py --dataset apolloscape --model trajectron --mode multi_frame --overwrite

Once the results are generated, paste the postProcessing.ipynb file in the test->data->dataset->trajectron_apolloscape->multi_frame location.

The postProcessing notebook looks for a .txt file called File_Names_Updated with the list of json file names you want to extract. A simple list contents command in shell will return these values from the attack->raw and normal->raw directories. Once that's set up, just go ahead and run the full notebook.

Reference links:
1. Formulated test cases and pretrained model for Trajectron++ from https://github.com/zqzqz/AdvTrajectoryPrediction/tree/master
2. Trajectron++ source code to generate input data for preprocessing prior to attack formulation - https://github.com/StanfordASL/Trajectron-plus-plus
3. Apolloscape Dataset - https://github.com/ApolloScapeAuto/dataset-api/tree/master/trajectory_prediction
