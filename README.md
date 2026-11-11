ICD 341 Labs 14–17: Assessment Question Answers
Answers to the assessment questions at the end of each lab. The PDF labels them Lab 1 to 4, but they belong to Labs 14 to 17.
Lab 14: EM Algorithm for Gaussian Mixture Models
1. EM algorithm: An iterative method for estimating model parameters when some information is hidden or missing. It alternates between an E-step and an M-step until the parameters stabilise (the likelihood stops improving).
2. Gaussian Mixture Model: A probabilistic model that assumes the data come from a mixture of two or more normal distributions. Each component has its own mean, variance and mixing proportion.
3. E-step vs M-step: The E-step uses the current parameters to compute the probability that each observation belongs to each component. The M-step uses those probabilities as weights to update the means, variances and mixing proportions.
4. Importance of clustering: It finds natural groups in unlabelled data. This helps with summarising data, segmenting populations (e.g. customers or farms), spotting patterns and supporting further modelling.
5. n_components: It sets the number of Gaussian distributions (clusters) the model should fit.
6. Importance of BIC: BIC compares models by balancing goodness of fit against complexity, penalising extra parameters. The model with the lowest BIC is preferred, which helps choose the number of components without overfitting.
7. fit(): It runs the EM algorithm on the data to estimate the means, covariances and weights of the model.
8. Applications of GMM: Customer segmentation, image segmentation, speech recognition, anomaly detection, and grouping crops or students by performance.
Lab 15: Neural Network with PyTorch Autograd
1. Neural network: A machine-learning model inspired by the brain. It consists of connected neurons arranged in input, hidden and output layers, and it learns patterns from data to make predictions or classifications.
2. PyTorch: A Python library for building and training machine-learning and deep-learning models. It provides tensors, automatic differentiation and neural-network modules.
3. Autograd: PyTorch's automatic differentiation feature. It tracks operations on tensors with requires_grad=True and computes gradients (derivatives) automatically.
4. Tensor: A multidimensional array of numbers, like a NumPy array, that also supports gradient tracking and GPU computation.
5. Loss function: It measures the difference between the model's predictions and the actual values (e.g. MSELoss). Training aims to minimise it.
6. Importance of gradient descent: It updates the parameters in the direction that reduces the loss, using the gradients. This is how the network learns.
7. backward(): It computes the gradients of the loss with respect to every parameter by backpropagation and stores them in .grad.
8. Optimizer: It uses the stored gradients to update the model parameters (e.g. SGD with a learning rate) through optimizer.step().
9. Training vs testing data: Training data is used to fit the model's parameters. Testing data is kept unseen and is used to evaluate how well the model generalises.
10. Applications: Predicting house prices, recognising handwritten digits, predicting customer behaviour, classifying agricultural products, and medical diagnosis.
Lab 16: Notebook Hygiene and Reproducible Packaging
1. Reproducibility: The ability of another researcher to use the same data, code and instructions to repeat an analysis and get the same or sufficiently similar results.
2. Notebook hygiene: Keeping Jupyter notebooks clean, organised and readable. That means a clear title, objectives, sectioned cells, explanations, correct outputs, graphs with interpretation, conclusions and references.
3. Random seeds: A seed (e.g. np.random.seed(123)) makes the random number generator produce the same sequence every run, so simulated results can be repeated.
4. nbconvert: A Jupyter tool that converts notebooks into other formats such as HTML, PDF and Python scripts.
5. Formats: HTML, PDF and Python script (.py). Markdown and LaTeX are also supported.
6. README file: It explains what the project is, how to install the requirements and how to run it, so others can understand and use it.
7. requirements.txt: It lists the Python libraries the project needs, so they can be installed with pip install -r requirements.txt.
8. Why organise project files: It makes the work easy to navigate, review, share and rerun. It reduces errors and lets a lecturer or collaborator find the data, code and outputs quickly.
9. CSV file: A Comma-Separated Values file is a simple text format for storing tabular data, with values separated by commas.
10. Importance of reproducible research: It builds trust in results, allows verification and error detection, supports collaboration and lets future work build on the analysis.
Lab 17: Interactive Dashboards with Streamlit
1. Dashboard: An interactive visual display that presents key information using graphs, tables and numerical summaries in one place.
2. Streamlit: A Python framework for building interactive web apps and dashboards from Python scripts, without web-development skills.
3. Panel: Another Python framework for building interactive dashboards and data applications. It is more flexible and supports many visualisation libraries.
4. Advantages of dashboards (any three): They make data easier to understand, let users interact with the data (filters and dropdowns), present results in one place, make findings easy to share and support quick decisions.
5. st.title(): It displays the main title at the top of the app.
6. st.dataframe(): It displays a pandas DataFrame as an interactive table that can be scrolled and sorted.
7. selectbox(): It creates a dropdown menu so the user can choose one option (e.g. a district). The app then shows information for that choice.
8. Data visualisation: Presenting data graphically (charts, plots, maps) so patterns, trends and comparisons are easier to see.
9. Static graph vs interactive dashboard: A static graph is a fixed image that cannot change. An interactive dashboard responds to user input (selecting, filtering) and updates what is displayed.
10. Applications: Monitoring crop production by district, tracking survey results or student performance, and exploring model outputs (e.g. cluster results or regression fits).
