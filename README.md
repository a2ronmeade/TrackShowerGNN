# TrackShowerGNN
GNN classification of track/shower clusters for DUNE LArTPC detectors, created as part of REU project for Aaron Meade, @ The University of Kansas, Summer 2026 w/ Dr. Maria Brigida Brunetti  

**SEE THE WIKI FOR MORE DETAILED INFORMATION**

**TrackShowerGNN.ipynb**: Notebook that includes pretty much the entire GNN project from top to bottom. Includes loading data, preprocessing, model training, optimization, model inference, analysis.  

**OptimalInference.ipynb**: Notebook designed only to run inferences on data and assign a probability score (`pTrack`) to clusters. Appends `pTrack` to root files organized the same way as the input data.  
* **OptimalModel-{tag}/checkpoints/best_model.pt**: Saved weights for the optimal model. File can be replaced to load in new weights, as long as hyperparamters in the model architecture are set to match the model which generated the pt file.

**environment.yml**: The environment that will be needed to run the model. (Essentially just lists what packages you'll need to have downloaded)
