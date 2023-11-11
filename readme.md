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

A sample json object of the schema is shown below. The entire sample json format and its corresponding schema are in the [schema folder of this repo](https://github.com/handlerda/accredited-investor-standard-schema/tree/master/schema)

```json
{
  "question": "Is it a family office and its family clients if the family office has assets under management in excess of $5 million and whose prospective investments are directed by a person who has such knowledge and experience in financial and business matters that such family office is capable of evaluating the merits and risks of the prospective investment?",
  "response": true,
  "originalResponseDateTime": "2022-01-12T12:00:00Z",
  "latestResponseDateTime": "2022-01-13T14:00:00Z",
  "summarizedQuestion": "Is it a qualified family office?",
  "additionalDetails": {
    "encodedDocument": [
      {
        "encoding": "base64",
        "type": "pdf",
        "value": "U29tZURvY3VtZW50YXRpb24="
      }
    ],
    "documentLink": [
      {
        "url": "https://example.com/document14",
        "type": "pdf"
      }
    ],
    "freeText": "Any additional text can be added here. Use a \n for a new line",
    "createdDateTime": "2022-01-11T12:00:00Z",
    "updatedDateTime": "2022-01-12T14:00:00Z"
  }
}
```

**Note on Complexity and Additional Details:**

For example:

- `"encodedDocument"` can store encoded versions of pertinent documents.
- `"documentLink"` can direct to a specific location within a document repository system.

Both of these elements are arrays of objects, enabling investors to have multiple supporting documents with unique file types. It's essential that the order of the array corresponds with the intended reading sequence of the documents. This approach guarantees that all relevant data, including primary documents or references, is organized and accessible within one comprehensive structure. Due to the intricate nature of these determinations, supporting context and documents are almost always necessary.

### Contribution

**We love your input! We want to make contributing to this project as easy and transparent as possible, whether it's:**

- Reporting a schema change.
- Discussing the current state of the code.
- Becoming a co-maintainer.
- Something else

**We Develop with Github**

We use GitHub to host code, to track issues and feature requests, as well as accept pull requests.

1. Fork the repo and create your branch from `master`.
2. If you've changed the schema, update the `readme.md` accordingly.
3. Make sure your code lints.
4. Issue your pull request!
