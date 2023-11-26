# Question_5_Viruses 

**Import the data for double-stranded DNA (dsDNA) viruses taken from the Supplementary Materials of the original paper into Posit Cloud (the csv file is in the question-5-data folder). How many rows and columns does the table have?**  
The data set provided for question 5 has 33 rows, and 13 columns.  

**What transformation can you use to fit a linear model to the data? Apply the transformation.**  
To fit a linear model, a logarithmic transformation should be used.  
<img width="464" alt="Screenshot 2023-11-26 at 12 31 48 pm" src="https://github.com/lanonmymoush/Question_5_Viruses/assets/151572854/3078bbc3-f3e2-48f7-9b36-b6d30e05a2c9">  

**Find the exponent (α) and scaling factor (β) of the allometric law for dsDNA viruses and write the p-values from the model you obtained, are they statistically significant? Compare the values you found to those shown in Table 2 of the paper, did you find the same values?**  
To find the exponent and the scaling factor, a linear regression should be used and summarised. The linear regression would compare the association between the variables log_genome_length and log_virion_length.  
<img width="525" alt="Screenshot 2023-11-26 at 12 42 08 pm" src="https://github.com/lanonmymoush/Question_5_Viruses/assets/151572854/ceb7bc1d-2ca5-424d-8784-aa5d793fc31c">  
The above image shows the summary table of the linear regression of log transformed variables, virion_volume and genome_length. The table shows the intercept- representing the scaling factor, and log_genome_length, representing the exponent. It can be seen that both values are highly significant. 
When compared to Table 2 of the Cui et al (2014) table 2, it can be seen that the values are similar.  
<img width="896" alt="Screenshot 2023-11-26 at 12 44 57 pm" src="https://github.com/lanonmymoush/Question_5_Viruses/assets/151572854/675c982c-2d23-40a0-a469-c3f76124ff25"> 
The exponent of 1.52 was found in my linear regression, as was the scaling factor of 1182 when the log-transformed value of 7.0748 is backtransformed (exp(7.0748) = 1181.807). 

**Write the code to reproduce the figure below**  
<img width="661" alt="Screenshot 2023-11-26 at 2 27 54 pm" src="https://github.com/lanonmymoush/Question_5_Viruses/assets/151572854/1fa596bb-80d9-4efe-8166-02241229c4ec">  
Code to produce the above figure provided in repository- "Question_5_Viruses.R". 

**What is the estimated volume of a 300 kb dsDNA virus?**  
To estimate the volume of the 300kb dsDNA virus, the initially provided equation would have to be used:  
<img width="74" alt="Screenshot 2023-11-26 at 3 08 32 pm" src="https://github.com/lanonmymoush/Question_5_Viruses/assets/151572854/5298a102-726e-4847-91b3-44aa212bde8c">  
Based on calculations, where β is the scaling factor, 1181.807, and α is the exponent, 1.52, the approximate virion volume for a dsDNA virus of 300kb appears to be 6697006 (approximately 6.7e+06). This could also be prone to variation due to the standard error of the calculation.  
<img width="107" alt="Screenshot 2023-11-26 at 4 10 36 pm" src="https://github.com/lanonmymoush/Question_5_Viruses/assets/151572854/adbcb754-0578-452d-9c3a-1c28af09169b">



