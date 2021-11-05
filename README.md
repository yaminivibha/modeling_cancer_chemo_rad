# modeling_cancer_chemo_rad
Modeling cancer cell growth and the effects of chemotherapy and radiation using ODE systems + exploring numerical methods for math modeling

One popular ODE model for tumor growth is based on the logistic equations. Rather than just modelling tumor growth as a logistic function, 
it introduces the interaction between tumor and normal cells as a factor influencing growth rates, as supported by cellular tumor research.

However, a newer model proposes the introduction of another factor: a simple immune system. 
To explore this model further, I will: 
(1) (a) implement a version of a logistic ODE model for tumor-normal-immune interactions, as laid out by Feizabadi et al 
    (b) explore a few test cases, observe model behavior
(2) explore the effects of different styles of ODE solvers: "hybrid", implicit, and explicit
(3) with the most computationally efficient solver, explore model kinetics with regard to how drug dosing changes tumor/normal cell behavior
(4) Investigate how drug resistance can be added into this system

With all this, I will improve my understanding of (a) ODE models for tumor growth, 
                                                  (b) immune system-tumor cell-normal cell interaction, 
                                                  (c) the effects of the design choices made in this model on its output
                                                  
                                                
                                                     
Mathematical models (particularly ODE models) can be a useful way to understand cancer tumor growth and development 
and particularly to make predictions about the efficacy of cancer treatments. 
It's certainly worthwhile to take a closer look at how those models are constructed, ESPECIALLY if they have real-world consequences 
such as determining which drugs might make it to FDA screenings etc.

Beyond that, selecting a solver for the model can have real effects on the reliability/error when running an ODE model
with regard to computation speed and accuracy, so it's worthwhile to investigate a few types of solvers to see what might suit this particular model. 

I personally am interested to explore parameters studies on this model as a way to better understand the design of the model with regard to how the parameters influence each other/interact. 

Last but not least, I take a look at a potential way of incorporating drug resistance for chemotherapy into the model. 
This is a real and particularly painful challenge in cancer treatment. 
I specifically look at physiological/mutation-based chemotherapy resistance to observe how it changes tumor and normal cell populations over time.                                                  
