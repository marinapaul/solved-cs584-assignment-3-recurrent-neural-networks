Download Link: https://assignmentchef.com/product/solved-cs584-assignment-3-recurrent-neural-networks
<br>



<ol>

 <li><strong>Language Modeling </strong>(100 points) In this homework, you need to implement a Recurrent Neural Network for language modeling with word embeddings on the Penn Treebank corpus. Please follow the steps as below:

  <ul>

   <li>(10pts) Preprocess the train and validation data, build the vocabulary, tokenize, etc.</li>

   <li>(10pts) Initialize parameters for the model.</li>

   <li>(20pts) Implement the forward pass for the model. Use an embeddings layer as the first layer of your network (i.e. nn.embedding lookup). Use a recurrent neural network cell (GRU or LSTM) as the next layer.</li>

   <li>(20pts) Calculate the loss of the model (sequence cross-entropy loss is suggested)</li>

  </ul></li>

</ol>

i.e. tf.contrib.seq2seq.sequence loss.

<ul>

 <li>(10pts) Calcuate the model’s perplexity (perplexity is number of predictionsexp(total loss) ).</li>

 <li>(10pts) Set up the training step: use a learning rate of 1<em>e</em>− 3 and an adam optimizer.</li>

 <li>(20pts) Train you model and report the perplexity (set window size to be 20, batch size to be greater than 1, e.g. 50).</li>

</ul>

Checking on your model: To check how your model is doing (and to actually see the cool thing your model is doing), we recommend, but are not requiring, looking at the sentences your model is generating. To do so, you can append together the argmax of the logit predictions after each sess.run() to create a generated sentence representation. You can then convert each word index to its corresponding English word from your vocab to create readable sentences.