# W&M DATA 340-03 Dataset Creation Overview

## Project Name 

Terms & Conditions Evaluator 

## Project Description

“Terms & Conditions from Financial Institutions and Social Media Platforms”. We've all accepted them but did we actually read them? 


## Sources of Data 
All data comes from companies' public web sites

* Truth Social 
https://help.truthsocial.com/legal/terms-of-service/
8012 words

* Facebook aka Meta
https://www.facebook.com/terms.php
Proving problematic

* Discord
https://discord.com/terms
7015 words

* Bank of America
https://www.bankofamerica.com/online-banking/service-agreement.go?request_locale=en-us
16815 words

* M&T Bank
https://www3.mtb.com/homepage/explore-the-m-and-t-bank-help-center/digital-services-agreement?ch=emld&cid=emld%7Cemail%7C133520%7C17638177%7C%7C
32253 words

* TransUnion
https://annualcreditreport.transunion.com/dss/termsOfUse.page?
2308 words

* Additional sources are being evaluated

All sources give consent for their terms of service to be read. 

At this point the corpus, a dataframe, could consist of multiple documents. One for each "terms of service". a single dataframe may not be the best way to represent the data. It may require a separate dataframe per site. 

Overall size will not be an issue. 

The evaluation would be mainly performed on each document stand alone.  Unclear of the value of TF-IDF for this but it will be calculated. 


## Challenges

Certain web pages are proving difficult to scrap. Rarely does a company actually place the readable text in the body of the html where it can be easily extracted. Of course, that's part of the NLP challenge. Certainly more complicated than eliminating punctuation or tokenizing. If needed it is hoped that they can be converted to PDF files and then read in.