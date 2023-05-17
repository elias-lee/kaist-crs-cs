<h1> KAIST_CRS_CS </h1>

<p> This is a repository for the paper "Machine Learning Driven Aid Classification for Sustainable Development"
Accepted to [IJCAI 2023: AI and Social Good Track](https://ijcai-23.org/) 


<p> Our research aims to create a text-classifier that automatically classifies the <b> purpose code </b> of the ODA projects in the CRS data based on the project descriptions. </p>

<p> We employed </p>

<ul>
  <li>Random Forest</li>
  <li>Text CNN</li>
  <li>BiLSTM</li>
  <li>BERT</li>
  <li>ELECTRA</li>
  <li>Top-3 ELECTRA</li>
  <li>Top-5 ELECTRA</li>
</ul>

<p>For BiLSTM and CNN, we used ReLU activation in prediction with the embedding size 300, hidden dimension 64, and 10 epoch. Adam optimizer was used with a learning rate of 0.001. The batch size was set to 512.
For BERT and ELECTRA, we used a 2-layer multilayer perceptron with ReLU activation as the prediction layer. The hidden dimension was set to 100, and Adam optimizer was used with a learning rate of 3e-5. </p>

<p> the Results as Below </p>

| Model         | Accuracy |
|---------------|----------|
| Random Forest | 74.71    |
| TextCNN       | 87.53    |
| BiLSTM        | 82.04    |
| BERT          | 89.96    |
| ELECTRA       | 89.71    |
| Top-3 ELECTRA | 95.75    |
| Top-5 ELECTRA | 97.05    |