# Secret Project 1

## Set up instructions

Set up LM Studio on your machine. If your PC allows it try and go for a Q4 model. 

@ Bav, the thing you need to do to get ipynb on your machine is to install anaconda. 

Then you can run 9pm.ipynb to interact with the LLM. 

There is however one pdf missing (atp_atks.pdf) you may have to find this manually!

## Things I have fixed overnight 

- I have found some alternative embeddings so that we no longer have to rely on huggingface. This seems to work well.
- Improved PDF reader. It now tends to keep words whole. Could do with some work to improve the chopping up (e.g. into sections), and removing filler texts like copyrights etc.
- I have removed the answers from the database queries. I found that this would return an irrelevant document based on a wrong answer, and the LLM was forced to provide a response based on this. So this has been improved at least.

## Things that I have tried and haven't worked. 
- Unfortunately googcolab didn't work so well for me.
- Varying the temperature, for some questions I had to set it high to get the right answer, for others I had to set it low.
- Max Tokens - for some, if you let it talk t0o long, the code that selects which option it is talking about struggles to find the correct match. But if you set it too short, it doesn't have time to say the right answer.
- Answers that are quite similiar (e.g. 49, A and C) the code that selects which option the LLM is talking about gets it completely wrong.


## To be done. 
- regardless of progress we need a script that runs over the whole question sets and answwers it.
- loading of all relevant pdfs
- then refine it so it actually gives correct answers, but the underlying functions are already in place. May need rewwriting entirely. 

