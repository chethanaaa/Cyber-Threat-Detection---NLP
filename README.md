# Cyber-Threat-Detection---NLP

*Introduction : *

According to the latest estimates, over 300 million terabytes of data are created every day and these numbers are increasing by the year as we witness more technological advancements. Ever since the proclamation that “The world’s most valuable resource is no longer oil, but data”, cyber attackers have been unrelenting in their attempts to seize this data for nefarious purposes. Much of this data existing on the cloud consists of text, often unstructured. Given NLP’s primary focus on extracting valuable insights from text data, there is a lot of potential in this field for mitigating cyber threats.

Text classification and entity recognition help extract insights and detect threats in cybersecurity. Upon detecting a threat, an NLP model can quickly search company data for malicious information. By analyzing keywords, context, and sentiment in forums, cybersecurity professionals can identify potential attacks before they occur. NLP algorithms can also flag anomalies in employee communication, indicating compromised accounts or insider threats. We aim to build a system to detect cyber threats from different communications channels and explain the cause for these cyber threats leveraging NLP techniques.

**Dataset and Features/Attributes: **

We have a cyber threat detection dataset containing diverse data types crucial for detection, diagnosis and mitigation of cyber threats. It comprises features such as textual content of 2-3 sentences containing descriptions of cyber threats, structured entries encapsulating sender IDs, threat labels and receiver IDs. Additionally, it includes relational data indicating entity relationships. We have 22 classes of potential cyber threats in 20k observations, half of which contain no labels/no threat detected.

**
Methodology:**

Models - we aim to leverage transformer based models such as BERT to perform these classification tasks.
BERT - excels in capturing bidirectional contextual information from text. It can effectively handle unstructured text data and is capable of tasks such as text classification
XLNet, RoBERTa, DistilBERT (employing distilled models for ease of training)

We aim to try either of 2 approaches:
Hierarchical modeling - frame the initial problem as a binary classification (threat / no threat) and add another layer of modeling which will create a probability distribution over the type of threat when one is detected from the 20 types of threats/classes.
Explainability - threat detection in addition to explaining the cause of a particular threat from the text.

Evaluation Metric:
We will use Accuracy, Precision, Recall, and the F1 Score, which are critical for assessing the model's performance in correctly identifying and classifying entities since we have a large number of classes. Confusion Matrix to provide a visual and quantitative representation of the model's performance across different classes. This metric will help us understand the model's discriminative power at various threshold settings, ensuring robustness in our predictive accuracy.
