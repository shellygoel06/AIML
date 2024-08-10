
Symantic Spotter using LlamaIndex.

Prerequisite to run the Symantic Spotter.

Step1. : Run all the cell in install all required library and depended code.


How to Run the Symatic Spotter: 

There are two ways.  you execute the query over list of insuracne documents. 

1. For sinle Query: you can directly pass the query to query_response method.  
Sample Query and Resposne:

Q: print(query_response("what is beneficiary in HDFC insurance policy?"))

Respone: 

The beneficiary in HDFC insurance policy is the individual or entity designated by the insured member to receive the benefits under the policy in the event of the insured member's death.
Check further at Copy of HDFC-Life-Group-Term-Life-Policy.pdf for document references.
Similarity score is :0.84421738104293

2. Using testing_pipeline method for multiple questions: 
Create a list of test questions and passed to testing_pipeline. it will ask for feedback please reposnd with good or bad. 

Sample Query and Resposne:
Q:
questions = ['what is beneficiary in HDFC insurance policy', 'Which is company name is talking about in provided context?',' who is eligible member in the context of insurance policy?',
             'when a person can recieve the claims?']
             
>testing_pipeline(questions):   

Response from Semantic Spotter:


he beneficiary in HDFC insurance policy is the individual or entity designated by the insured member to receive the benefits under the policy in the event of the insured member's death.
Check further at Copy of HDFC-Life-Group-Term-Life-Policy.pdf for document references.
Similarity score is :0.8327875397728577

 Please provide your feedback on the response provided by the bot
good
Answer  from cache:

Which is company name is talking about in provided context?
Answer from LLM:

HDFC Life
Check further at Copy of HDFC-Life-Group-Term-Life-Policy.pdf for document references.
Similarity score is :0.7607341495571885

 Please provide your feedback on the response provided by the bot
goos
Answer  from cache:

 who is eligible member in the context of insurance policy?
Answer from LLM:

An eligible member in the context of the insurance policy is a person who satisfies the eligibility criteria mentioned in the policy and is aged less than the Benefit Expiry Age.
Check further at Copy of HDFC-Life-Group-Term-Life-Policy.pdf for document references.
Similarity score is :0.8300824845796103

 Please provide your feedback on the response provided by the bot
good
Answer  from cache:

when a person can recieve the claims?
Answer from LLM:

A person can receive the claims after submitting all necessary claim documents within 60 days from the date of diagnosis of the condition. However, the delay in claim intimation may be condoned if valid reasons are provided for the delay.
Check further at Copy of HDFC-Life-Easy-Health-101N110V03-Policy-Bond-Single-Pay.pdf for document references.
Similarity score is :0.8129318553758091

 Please provide your feedback on the response provided by the bot
good
Answer  from cache:

Question	Response	Good or Bad
0	what is beneficiary in HDFC insurance policy	The beneficiary in HDFC insurance policy is th...	good
1	Which is company name is talking about in prov...	HDFC Life\nCheck further at Copy of HDFC-Life-...	goos
2	who is eligible member in the context of insu...	An eligible member in the context of the insur...	good
3	when a person can recieve the claims?	A person can receive the claims after submitti...	good








