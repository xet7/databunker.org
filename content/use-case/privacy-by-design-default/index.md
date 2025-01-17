---
title: Privacy by design compliance out of the box
summary: Privacy by design is about considering data protection and privacy issues upfront in everything you do.
abstract: ""
weight: 50
authors: []
tags: []
type: docs
mymenu: usecase
featured: false
image:
  caption: 'Image'
  focal_point: Right

links:
#- icon: twitter
#  icon_pack: fab
#  name: Follow
#  url: https://twitter.com/georgecushen
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects:
# - internal-project
---
One of the important trends of modern software development is **privacy by design** and **privacy by default** principles.

**Privacy by design** stands that organizations should consider data protection issues as part of the design and implementation of systems, services, products, and business practices.

The GDPR requires you to integrate **data protection** concerns into every aspect of your processing activities. This approach is **data protection by design and by default**.

In this article, we’ll be taking an in-depth look at the **privacy by design** principle and how to achieve it with simple steps.

I will talk about an open-source product our team develops called **Databunker** and how it can help.

Databunker is an open-source secure vault for customer records built with the **privacy by design** principle. This product brings **compliance out of the box** for any company implementing Databunker. Databunker can serve as a cornerstone for your privacy by design solution.

## Privacy By Design Actionable Plan.

The following is a partial list of actionable plans to make your business **privacy by design** compliant.
### 1. Create a map of personal data flows and processing operations.

For GDPR compliance, your company should map every moment of the personal data lifecycle. The company must know what happens to personal data, why and if any external parties are involved. You need to identify all 3rd party services that have even access to the personal data including access to partial data.

Ensure that any data processor your company is using also implements appropriate technical and organizational measures for personal data security.

### 2. Identify the lawful basis for the processing of personal data.

You need to have a legal basis **before** processing personal data. For example in can be in a form of **consent**. **Cookie popup** is one example. Another alternative is to update the privacy policy, terms of service, or a company's contract.

Consult with the lawyers at this step.

### 3. Update privacy policy and terms of service documents.

With your privacy policy you need to address the following:
1. Make sure your customer knows what 3rd party companies you are using to process personal data. For example what CRM service you use.
1. You need to help your customers with the execution of their user rights. You need to provide an active email address to send all user requests.
1. If you need to do cross-border personal data transfer, you can detail it here.

Consult with the lawyers at this step.
### 4. Minimize personal data.

You need to minimize the personal data your business collects. A general rule for you is to keep personal data at minimal only required to perform the business and remove all unused data. You need to do it to comply with **data minimization** and **storage limitation** GDPR principles. 

One of the results of this rule is that you need to remove personal data for expired trial customers of customers that left the company service.

**Databunker** can be used for secure personal data storage. Check this article for additional information: https://databunker.org/use-case/data-minimization/

## 5. Best practice of personal data encryption and encryption of app session data.

GDPR stands on **integrity and confidentiality** as leading principles. These principles tell that appropriate security measures should be in place to protect personal data.

Although there are **no explicit GDPR encryption requirements**, the regulation does require you to enforce security measures and safeguards. The GDPR repeatedly highlights **encryption** and **pseudonymization** as “**appropriate technical and organizational measures**” of personal data security.

**Databunker** stores your customer's personal data in an encrypted manner and builts a secure index to search for personal records. In addition Databunker supports [session data encryption and storage](https://databunker.org/use-case/secure-session-storage/).

## 6. Personal data pseudonymisation.

**Pseudonymisation** is a perfect solution for cross-border personal data transfer. When saving a user object in Databunker you are getting a **user token**. This user token is a user's **pseudonymized identity**. When performing a cross-border transfer, change user personal data with a **user token** generated by **Databunker**.
**Pseudonymisation** helps with storing logs: https://www.freecodecamp.org/news/how-to-stay-gdpr-compliant-with-access-logs/

## 7. Data protection awareness training.

You can use our training for your personal. Use the following link: https://basebunker.com/

## 8. Audit sensitive operations - accountability principles.

It is a key element of the GDPR’s risk-based approach and its focus on accountability, i.e. your ability to demonstrate how you are complying with its requirements.

**Databunker** can keep track of any operation with personal data.

## 9. Cross-border personal data transfer

Cross-border personal data transfer is an extremely important aspect of GDPR. Especially with the invalidation of the **Privacy Shield Framework**. This framework was used by 5,000 U.S. companies to conduct trans-Atlantic trade in compliance with EU data protection rules. The reason behind this decision is that the current level of protection given to personal data under US law cannot be considered to be the same provided by the European Union. This is largely due to US surveillance programs.

Today, you have a number of solutions to do the cross-border transfer.
1. The first is to use **Standard Contractual Clauses (SCC)**. It is also known as **Model Clauses**. It means you users need to approve for their personal data processed abroad, for example in the US. It can be done for example if your user gives you explicit consent. 
2. Another solution is to use European Data Protection Board (EDPB) guidelines (2020). This document details a number of technical solutions for cross-border transfer. One of the methods is pseudonymization covered before.

## 10. Make your app logs privacy compliant

There are several methods to make your logs privacy compliant. For example, using **pseudonymization**. Check the following article for additional information: https://www.freecodecamp.org/news/how-to-stay-gdpr-compliant-with-access-logs/

# Additional steps:
1. Data confidentiality, integrity, and availability.
1. You must have appropriate security to prevent the personal data you hold from being accidentally or deliberately compromised.
1. Keep track of any operations with PII.
1. Cookie popup.
1. Cross-border personal data transfer
