# Accredited Investor Criteria README

This document provides an overview of various questions and criteria that determine whether an entity or individual qualifies as an accredited investor. Each item has a summarized version for quick reference.

## Benefits

**The Importance of a Standard Schema for Accreditation and its Utility in Document Prepopulation**

When various entities in the financial and legal sectors agree on a standardized schema for accreditation, it paves the way for enhanced efficiency and utility:

1. **Lawfirms**: Adopting a standard schema simplifies the drafting and review process. Documents can be easily prepopulated with relevant investor information, ensuring accuracy and saving valuable time. This not only accelerates transactions but also reduces the risk of manual errors. Furthermore, a uniform schema allows law firms to utilize advanced document automation tools, streamlining their services across various clients and investment opportunities.

2. **Electronic Signature Companies (e.g., Docusign, Adobe Sign)**: With a standard schema in place, these platforms can more seamlessly integrate and prepopulate accreditation data in documents awaiting electronic signatures. This ensures that every signed document is both consistent and compliant, further enhancing the reliability of electronic transactions.

3. **Accredited Investors**: For investors, the ability to have documents prepopulated based on a standard schema minimizes repetitive tasks. They can quickly review and sign investment documents, knowing that their essential details are already accurately integrated. This not only expedites their investment process but also provides them with a more user-friendly experience.

Incorporating a standard schema for accreditation, thus, not only ensures clarity and consistency but also introduces a level of automation in document preparation. This benefits all stakeholders by optimizing processes, reducing errors, and ultimately fostering a more streamlined and efficient investment ecosystem.

## Criteria

The presented table provides a concise summary of the criteria that define an "accredited investor" as outlined in [Section 230.501 of the Electronic Code of Federal Regulations (eCFR)](https://www.ecfr.gov/current/title-17/chapter-II/part-230/subject-group-ECFR6e651a4c86c0174/section-230.501). This section, found on the official eCFR website, enumerates the various qualifications and conditions an entity or individual must meet to be considered an accredited investor under U.S. securities laws. By distilling the intricate legal language of the eCFR into a clear and organized table format, we aim to offer a more accessible and straightforward reference for stakeholders and developers.

| **Criteria Number** | **Summarized Question**                                              | **Detailed Question**                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | -------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1                   | Is it a financial institution?                                       | Is the entity a bank, savings and loan association, insurance company, registered investment company, business development company, or small business investment company or rural business investment company?                                                                                                                                                |
| 2                   | Is it a registered financial adviser?                                | Is the entity an SEC-registered broker-dealer, SEC- or state-registered investment adviser, or exempt reporting adviser?                                                                                                                                                                                                                                      |
| 3                   | Is it a state employee benefit plan with assets over $5 million?     | Is it a plan established and maintained by a state, its political subdivisions, or any agency or instrumentality of a state or its political subdivisions, for the benefit of its employees, if such plan has total assets in excess of $5 million?                                                                                                           |
| 4                   | Is it an ERISA plan with assets over $5 million?                     | Is it an employee benefit plan (within the meaning of the Employee Retirement Income Security Act) if a bank, insurance company, or registered investment adviser makes the investment decisions, or if the plan has total assets in excess of $5 million?                                                                                                    |
| 5                   | Is it a large tax-exempt organization or corporation?                | Is it a tax-exempt charitable organization, corporation, limited liability corporation, or partnership with assets in excess of $5 million?                                                                                                                                                                                                                   |
| 6                   | Is the individual an officer or director of the selling company?     | Is the individual a director, executive officer, or general partner of the company selling the securities, or any director, executive officer, or general partner of a general partner of that company?                                                                                                                                                       |
| 7                   | Are all equity owners accredited investors?                          | Is it an enterprise in which all the equity owners are accredited investors?                                                                                                                                                                                                                                                                                  |
| 8                   | Is the individual's net worth over $1 million?                       | Is the individual's net worth or joint net worth with a spouse or spousal equivalent at least $1 million, not including the value of his or her primary residence?                                                                                                                                                                                            |
| 9                   | Does the individual have high income?                                | Does the individual have income exceeding $200,000 in each of the two most recent calendar years or joint income with a spouse or spousal equivalent exceeding $300,000 for those years and a reasonable expectation of the same income level in the current year?                                                                                            |
| 10                  | Is it a knowledgeable trust with assets over $5 million?             | Is it a trust with assets exceeding $5 million, not formed only to acquire the securities offered, and whose purchases are directed by a person who meets the legal standard of having sufficient knowledge and experience in financial and business matters to be capable of evaluating the merits and risks of the prospective investment?                  |
| 11                  | Is it a non-traditional entity with over $5 million in investments?  | Is it an entity of a type not otherwise qualifying as accredited that owns investments in excess of $5 million?                                                                                                                                                                                                                                               |
| 12                  | Is the individual licensed in securities?                            | Is the individual holding in good standing any of the general securities representative license (Series 7), the investment adviser representative license (Series 65), or the private securities offerings representative license (Series 82)?                                                                                                                |
| 13                  | Is the individual a knowledgeable employee of a private fund issuer? | Is the individual a knowledgeable employee, as defined in rule 3c-5(a)(4) under the Investment Company Act, of the issuer of securities where that issuer is a 3(c)(1) or 3(c)(7) private fund?                                                                                                                                                               |
| 14                  | Is it a qualified family office?                                     | Is it a family office and its family clients if the family office has assets under management in excess of $5 million and whose prospective investments are directed by a person who has such knowledge and experience in financial and business matters that such family office is capable of evaluating the merits and risks of the prospective investment? |

## Sample JSON object

We suggest going the the /schema section to review the entire sample json format in addition to its corisponding schema. A sample json object is below for reference:

```json
{
  "question": "Is the individual a knowledgeable employee, as defined in rule 3c-5(a)(4) under the Investment Company Act, of the issuer of securities where that issuer is a 3(c)(1) or 3(c)(7) private fund?",
  "response": true,
  "originalResponseDate": null,
  "latestResponseDate": null,
  "summarizedQuestion": "Is the individual a knowledgeable employee of a private fund issuer?",
  "additionalDetails": {
    "base64EncodedDocument": null,
    "documentLink": null,
    "freeText": "relevant free text \n should be used to indicate a new line",
    "createdDate": null,
    "updatedDate": null
  }
}
```

**Note on Complexity and Additional Details**: The provided JSON structure can capture intricate details regarding the qualifications of an individual in the context of § 230.501. Given the complexity of such determinations, the "additionalDetails" section is crucial. It offers the capability to embed further related information. For instance, the "base64EncodedDocument" can be used to store encoded versions of relevant documents, while "documentLink" can point to a specific location in a document repository system. This ensures that all pertinent data, including primary documents or references, can be accessed or stored within a single, organized structure. Given the complexity of these questions supporting context and documents are nearly always required.
