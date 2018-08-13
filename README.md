# cmhn-s18-wk12-final
This is the repo for the default option of the final project. If you are doing this option, please complete the assignment by commiting changes to this repo. Please provide your final answer to each question in the original question notebook. In addition, you must show your work by providing code that generates this answer. This code should be placed in a separate file or set of files for each question, clearly labeled and referenced along with your answer in the question notebook. You are encouraged to commit your changes regularly (good practice in software development), however please make sure that your last commit contains only those files being used in generating the final solution.

*Instructor's corner*

Feedback:

**Question**  

Really interesting, novel and well motivated question  

**Apporach**  

This is really great, my comments are small in comparison. Great introduction.  
Your motivation for doing parcellation is missing a step in logic: if function doesn't map on to anatomy at the voxel level, why does it map on at the parcellation level?  
For the sliding window correlation analysis in step 4, 10 TRs is quite small. It would have been good to see a few other window sizes. Also for this analysis, it would be good to plot these correlation values to get a better feel for what is going on, this is a very dense section.  
Nice conclusion to this section, but it could be more thorough.  
You say you use FCMA to avoid potential issues with averaging over parcellations; however, what you do is not FCMA. For one, this isn't a full correlation matrix (you take every 3) but more importantly, you don't perform classification with the correlation matrices you create, which is a fundamental feature of FCMA.  
Brilliant work on the permutation analyses, these are really sophisticated! I would have loved to see these clusters back into brain space but I know that is hard. Really great conclusion, good job.  

**Clarity**  

Overall pretty clear but a few omissions.  
You don't provide any description of the dataset. Since the goal of this exercise is to make reproducible code, this is a big problem. Because of this, you also don't provide a rationale for why you chose that data.  
The definitions you create are not clearly commented. In general your code should be commented more and you should have a conclusion/discussion after every big code block (or better yet, smaller comments dispersed throughout).  
For the functions that are shared between notebooks, it may have made sense to make a Utils function that can be loaded by each one separately.  
You should have at least a short docstring describing what each function does and ideally a description of the inputs and outputs.  
For step 4, it would be good to plot the sliding window correlation values to get a better feel for what is going on, this is a very dense section. Also you should unpack the results of the affinity propogation.  
It would be good for you to discuss the results of step 6, why are there spikes in the affinity propagation for this analysis? That seems promising.

**Bonus**
Bonus awarded for Affinity propagation and Markov modeling
