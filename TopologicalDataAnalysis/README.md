# TopologicalDataAnalysis

 `Topological Data Analysis` is a data analysis and data visualization tool that has its roots in combinatorial topology. The `Stability Theorem` in `Persistent Homology` roughly states that "close" point cloud data have "close" `Persistence Diagrams`. Therefore, in the directory `RTDA` I computed the `Wasserstein Distance` between persistence diagrams of samples drawn from the same dataset. It uses the packages

1. `TDA` - https://cran.r-project.org/web/packages/TDA/
2. `TDAstats` - https://cran.r-project.org/web/packages/TDAstats/

In the directory `PythonTDA` I have used the package `Giotto-tda` - https://github.com/giotto-ai/giotto-tda for a few `Topological Data Analysis` use cases.

1. In `BreastCancerAnalysisViaTDA.ipynb` I performed breast cancer analysis as follows:

    1. Computed `VietorisRipsPersistence` based on the features of the breast cancer dataset.
    2. Used `PersistenceEntropy` to encode the features in an abstract form.
    3. Used the encoded features to train a `random forest` model to predict breast cancer.

2. In `KMapperDataVisualization.ipynb` I used `Kepler Mapper` (consult https://kepler-mapper.scikit-tda.org/en/latest/) to visualize the breast cancer dataset.

3. In `TimeSeriesTDA.ipynb` I computed and visualized the `persistent homology` in low dimensions of the `Apple Stock Price` time series dataset.