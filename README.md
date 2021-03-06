# Summarization in a tick of time!

Summarization is a process of shortening the whole context of a document to a short sentence or sentences. Here we use the natural language process techniques to create a summary of the given data. More information can be found in this blog: https://medium.com/@rahulmadan_18191/summarizations-in-a-tick-of-time-nlp-1d536d937357

We compare the summarizers performance using the various nlp models for the given data:
1. In Extractive Summarization we use the models like:
  - Bert
  - XL Net
  - GPT2
  - GPT3 - yet to be implemented
  
2. And, in Abstractive Summarization we use models like:
  - Bart
  - T5
  - PreSumm - yet to be implemented

follow to below steps to see the code running:
1. Clone the repo:
```
git clone
```
2. Intall the requirements file
```
pip install -r requirements.txt
```
3. Run the file
```
python sum_file.py
```
4. Ouptut:
```
If you are not born with the blue eyes, to obtain blue eyes naturally is not possible. There are many type of laser surgeries in the market which can change the colour of your eye to blue. In the special type of surgery, Dr burn the lower layer of melanin in your eyes.
[{'rouge-1': {'f': 0.1920289837713322, 'p': 1.0, 'r': 0.1062124248496994}, 'rouge-2': {'f': 0.18545454374241324, 'p': 0.9807692307692307, 'r': 0.10240963855421686}, 
'rouge-l': {'f': 0.3083333307253473, 'p': 1.0, 'r': 0.18226600985221675}}]
```

### Model Parameters:

The file - Summarization.py within folder Summarizer can be tuned for model or parameter change. the parameters can be changed at the following blocks: 

1. In Xlnet and GPT2
  - transformer_type
  - transformer_model_key
2. In Bart and T5
  - model
  - pipeline (more information on this can be found in this blog: https://medium.com/analytics-vidhya/nlp-pipelines-in-a-single-line-of-code-500b3266ac7b)
   
   
   Please rate a star if you find this repo useful! 

---------------------------------------------------------------

## References:
 - HF - Pipelines: https://huggingface.co/transformers/main_classes/pipelines.html
 - Summarizers pkg: https://github.com/michigan-com/summarizer
