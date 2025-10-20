# Enhancing Loss Reserving with Predictive Analytics: Linear vs Ensemble models datasheet

## 

## Motivation

This dataset was created so it can be used for claims reserving studies.

It was created by Glenn Meyers and Peng Shi under the sponsorship of the Casualty Actuarial Society (CAS).



## Composition

The dataset contains of insurer-level loss development triangles across 6  lines of business, with thousands of instances overall. 

Some missing values exist due to some insurers not writing a line of business and also some insurers had incomplete triangles due to reporting changes.

The dataset contains no confidential or personal data—only aggregated, regulatory financial information

## 

## Collection process

The dataset was collected by extracting insurer-level loss development information from the NAIC Schedule P regulatory filings. 

The strategy to collect the data was deliberate squaring of triangles across multiple years to provide both training and validation data for research.

The dataset covers accident years 1988 through 1997, with development observed through 2006. 

## 

## Preprocessing/cleaning/labelling

As mentioned earlier, the dataset went through significant preprocessing and cleaning before release. This was represented by the way the creators extracted the data from the NAIC Schedule and then squared them to standardise them across all insurers and lines of business before undergoing quality checks.

No advanced labeling like tokenization or feature extraction was needed, since the data is numeric and structured.

## Uses

Beyond claims reserving research it can be used for capital allocation and risk management for insurers otherwise known as portfolio optimisation.  It can also be used for comparative studies where researchers can compare loss development patterns across different lines of business.

The dataset was aggregated meaning that it can be prone to biased conclusions since only certain lines of business where selected, certain insurers and so forth. It could be heavily risky to apply the findings of this study to a sports insurance business as they are not related.

Understanding the context and purpose of the dataset is a way for someone to mitigate these risks. In addition, since this study was based on claims data over 30 years ago, it would be worthwhile to use a more up to date dataset in order to validate findings of this study even further and for it to be able to applied to modern day insurance claims.

This dataset should not applied for individual policy guidance, as this may lead to unfair treatment against the policy holder due to the dataset being aggregated.

## Distribution

The dataset has been distributed by the Casualty Actuarial Society (CAS) through its website, with permission from the National Association of Insurance Commissioners (NAIC). 

It is subject to the NAIC’s intellectual property rights and is made available under the CAS’s research resources with applicable terms of use of research and education purposes to not be distributed.

## Maintenance

The dataset is maintained by the Casualty Actuarial Society (CAS), on it's website - https://www.casact.org/publications-research/research/research-resources/loss-reserving-data-pulled-naic-schedule-p



