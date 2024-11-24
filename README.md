# Trustful and Reliable Spam Email Detection

## Methodology
### Classifier
A Random Forrest Classifier is trained on the Enron Spam/Ham Dataset.

### Explainer
A Shap Explainer is trained to output shap values for the Classifier model.

### Human Readable Explanation
Using the Shap Values, the top 10 words are filtered based on their contribution to the decision made by the classifier model.
These words are then, fed to Llama 3 along with their confidence score and alignment.
The LLM returns an explanation as to why the model made the decision that it did.
