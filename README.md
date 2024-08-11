# Neural_Networks_OCR

This was a workshop conducted under IEEE SIES GST, Focuses on understanding the core principles of Machine Learning. Here we covered concepts from basic Math used in computing a neuron to classifying 10 digit numbers using a fully connected Neural Network.under guidane of @Adityadikonda10

Lets start with computing output of a single neuron. the formula goes as:
neuron output=input⋅weight+bias

Now, lets compute multiple neurons at once, also known as a layer of neurons.
output=∑i=0n(inputi⋅weighti)+biases 

Here input and weight are arrays of float values of which dot product is calculated.

ReLU Activation Function.
ReLU(x)=max(0,x) 

ReLU is mostly used to activate hidden layers.

SoftMax Activation
Softmax(zi)=ezi∑jezj

Loss Calculation (Categorical Cross-Entropy)
Loss=−∑iyilog(pi)

Loss Calculation (Categorical Cross-Entropy)
Loss=−∑iyilog(pi)

Adam Optimizer
Compute the biased first moment estimate  mt 
mt=β1⋅mt−1+(1−β1)⋅gt 

where  gt  is the gradient at time step  t .
Compute the biased second raw moment estimate  vt :
vt=β2⋅vt−1+(1−β2)⋅g2t 

Compute bias-corrected first moment estimate  m^t :
m^t=mt1−βt1 

Compute bias-corrected second raw moment estimate  v^t :
mt=β1⋅mt−1+(1−β1)⋅gt 

Update the parameters  θ :
θt=θt−1−α⋅v^tm^t−−−√+ϵ
