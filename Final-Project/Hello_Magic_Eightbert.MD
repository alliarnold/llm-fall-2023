# Hello, Eightbert!

## *how are you today? **Outlook good**

### Intro

Magic Eightbert™ is a fine-tuned BERT model here to answer the questions on your mind today! Just kidding! Magic Eightbert doesn't have the answers, but that is why it is here —to help demonstrate the difference between probability-based responses and a time-machine-backed glimpse into the future.

### Premise

AI and other machine-learning tools are the shiniest toys on the market today, promising everything from the end of humanity as we know it to a solution for all our problems. Think pieces and government groups are reasonably dedicating a lot of time and research to considering how much labor, decision-making, and trust should be given to LLMs and other machine-learning tools, especially as we try to create an optimal future for humankind. 

Those of us who have had the privilege of studying statistics or the basics of machine learning should already have absorbed something that many people haven't. Having seen data converted into predictions, weights, and probabilities, we understand that LLMs are only as good as their architecture and training data, or "ground truth" as it is so generously misnamed. 

The reality is that humans collectively agree on very little about what is empirically true, particularly with issues that have major moral or societal implications. The next logical step in accepting this is to accept that no LLM in existence today was trained with 100% true capital "T" information. Whether or not you believe in AI hallucinations or see every output an LLM produces as equally hallucinogenic, the outputs provided by LLMs are no more and no less than a result of their design and input data. Predictive machine learning does not predict futures that haven’t happened already, it predicts what is most likely to happen again given the data provided. Sure, you can adjust certain frequencies to increase the randomness of your outputs, but that randomness is psychotic, not psychic.

### Concept

So, how do we explain something as complicated as neural network coding to someone who doesn’t code and hasn’t studied statistics? Oversimplification, of course! And that's where Magic Eightbert comes in. Many Americans of a certain age remember the old fortune-telling toy, the Magic Eightball. All the rage when it first came out, the toy found nary a true believer in its soothsaying abilities. Perhaps that is because it is a plastic toy with a viewing window revealing a floating four-sided die inside. The original Magic Eightball shows its work! With each shake of the ball, users can see the direct impact of their jostling of the toy as the floating die reacts to the user’s movement with an immediate and random roll before it ceases spinning to reveal a final side of the die with an answer, "Outlook good"!

Maybe we don’t know how to build our own Magic Eightballs, but generally, we understand how casting a die works. We can see the impact of our input (the shake) as different from our question, and we can see the answer on the die as a result of randomness mixed with the strength and duration of the shake inflicted, with a one in four chance for any answer. Maybe if we’re feeling particularly poetic we can even jump to imaging a comparison between a floating pyramidal die in water and a weighted word vector floating in multi-dimensional space too complicated for the human brain to fully visualize. Either way, we get it. We pose a question to a machine, and the probability of the dice gives us an answer. And that, my friends, is a vast oversimplification of an LLM. We submit our question to an LLM chatbox, it pulls all the weights in its architecture, bounces around the training data, and lands on the most likely crevasse on your kitchen table or browser.

## Approach

I used two custom datasets to train Magic Eightbert. Each dataset included one column of potential questions that someone might pose to a traditional Magic Eightball and a second column with corresponding answers. The first dataset assigned each question with one of the four original answers found on Magic Eightballs. For more fun and a greater variety, the second dataset assigned those same questions with one of any of the twenty total answers available in the later generations of the Magic Eightball.

Given the LLM of it all, I tried to use ChatGPT to draft the 1,000 questions, but the results were wildly repetitive. I ultimately edited the ChatGPT questions beyond recognition to create the final set. To ensure that BERT could be properly fine-tuned and learn from the training data, I established some consistency for applying answers —or my own entirely subjective moral code. I selected negative answers to respond to any questions relating to cruelty or lawbreaking (ex. should I kick puppies?, should I rob a bank?). For questions relating to the body, I generally assigned noncommittal answers, like “Cannot predict.” For questions relating to generosity (ex. should I give more money to charity?, should I volunteer?), I assigned positive answers. I also selected noncommittal answers for the majority of questions about what will happen in the future or major financial decisions.

In the end, I used that data to make two fine-tuned BERT models, with 10 epochs of learning each. Magic Eightbert™ 1.0 offers four possible answers and Magic Eightbert ™ 2.0 offers twenty.  Both models share the same general moral code which is somewhat inconsistently applied, but still visible through interacting with either model. The benefit of the moral code is twofold. One it allowed faster growth in accuracy between training epochs, and secondly it allowed me to put some bumper rails on Eightbert, ensuring that if anyone was full-hearty enough to take the advice, it was less likely to cause a damaging outcome. 


## Implementation

I hope that playing with Magic Eighbert can highlight LLMs’ dependence on probabilities and training data for folks who haven’t previously considered machine learning builds. Moreover, I want to show how LLMs can be fun and sometimes useful arrows in the right direction, but shouldn’t be depended on for accuracy or visions into the future.
