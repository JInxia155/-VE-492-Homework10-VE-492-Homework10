
Download Link : https://programming.engineering/product/ve-492-homework10/

# -VE-492-Homework10-VE-492-Homework10
 🔍 VE 492 Homework10 VE 492 Homework10

Question 1: Rejection Sampling

We will work with a Bayes’ net of the following structure.

In this question, we will perform rejection sampling to estimate P(C=1|B=1,E=1). Perform one round of rejection sampling, using the random samples given in the table below. Variables are sampled in the order A,B,C,D,E. In the boxes below, choose the value (0 or 1) that each variable gets assigned to. Note that the sampling attempt should stop as soon as you discover that the sample will be rejected. In that case mark the assignment of that variable.

When generating random samples, use as many values as[0,1)needed from the table below, which we

generated independently and uniformly at random from . Use numbers from left to right. To sample a binary variable W with probability P(W=0)=p and P(W=1)=1-p using a value from the table, choose W=1 if a<p and W=0 if a>=p

Enter either a 0 or 1 for each variable that you assign a value to. Upon rejecting a sample, enter its assigned value, and leave the fields for the remaining variables blank (use “b” for blank). For example, if C gets rejected, fill in “b” for D and E.

A____B____C____D____E____

Which variable will get rejected? If no variables will get rejected, leave the field below blank.

____

Sample answer:

01bbbB

Question 2: Estimating Probabilities from Samples

Below are a set of samples obtained by running rejection sampling for the Bayes’ net from the previous question. Use them to estimate P(C=1|B=1,E=1) . The estimation cannot be made whenever all samples were rejected. In this case, input -1.

Sample answer:

0.2

Question 3: Likelihood Weighting

We will work with a Bayes’ net of the following structure.

In this question, we will perform likelihood weighting to estimate . Generate a sample and its weight, using the random samples given in the table below. Variables are sampled in the order . In the table below, select the assignments to the variables

When generating random samples, use as many values as[0,1)needed from the table below, which we

generated independently and uniformly at random from . Use numbers from left to right. To sample a binary variable W with probability P(W=0)=p and P(W=1)=1-p using a value from the table, choose W=1 if a<p and W=0 if a>=p

Question 4: Estimating Probabilities from Weighted Samples

Below are a set of weighted samples obtained by running likelihood weighting for the Bayes’ net from the previous question. Use them to estimate P(C=1|B=1,E=1). Input -1 in the box below if the estimation cannot be made.

____ (Keep 2 decimal places)

Sample answer:

0.25

Question 5: HMMs, Part I

Consider the HMM shown below.

The prior probability

t

0) , dynamics model

t

1

) , and sensor model

t

) are as follows:

We perform a first dynamics update, and fill in the resulting belief distribution

t

1).

    1
    	

    )

    t

    1
    	

    , and the
    		

    1
    	

    		

    t

    1
    	

    )
    	

    t

    1

    )
    	

    evidence
    			

    . We fill in
    	

    We incorporate the
    			

    the evidence-weighted distribution
    	
    			

    (normalized) belief distribution
    		

    .
    	

Note: Please write your answer for each table in one row, that is, there will be 3 rows for this question. Besides, please use values rounded to 3 decimal places.

Sample Answer:

0.160,0.170

0.200,0.211

0.222,0.180

    You get to perform

the

)second dynamics update. Write your answer to fill in the resulting

belief distribution .

    					

    t

    )
    							
    		

    0
    										
    		

    1
    										
    						

    ,
    	

    		

    t

    )
    	
    					

    t

    )

    t

    )
    					

    2) Now incorporate the evidence
    					

    . Write your answer to fill in the evidence-weighted
    		

    distribution
    			

    and the (normalized) belief distribution
    		

    .
    				

    t

    )

    t

    )
    					
    					
    		

    0
    										
    												
    		

    1
    										
    												

Question 6: HMMs, Part II

Consider the same HMM.

The prior probability

t

0) , dynamics model

t

1

) , and sensor model

t

) are as follows:

    In this question we’ll assume the sensor is broken and we get no more evidence readings. We are

    t
    	

    )
    			

    , our belief about
    	

    forced to rely on dynamics updates only going forward. In the limit as
    	

    should converge to a stationary distribution
    	

    defined as
    	

    follows:
    	
    	

    	

Recall that the stationary distribution satisfies the equation

for all values in the domain of

.

In the case of this problem, we can write these relations as a set of linear equations of the form

In the spaces below, fill in the coefficients of the linear system. The system you have written has many solutions (consider (0,0), for example), but to get a probability distribution we want the solution that sums to one. Write your answer to fill in the table below.

(Hint: to check your answer, you can also write some code and run till convergence.)

Note: Please write your answer for each table in one row, that is, there will be 2 rows for this question. Besides, please use values rounded to 3 decimal places.

0.200,0.211
		
	

coefficient
	

value

a
		

b
		

c
		

d
		

0
		
	

t
	

)
		

1
		
		

