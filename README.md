## Overview

The Supply Chain Integrity Model (SCIM) supports the ongoing verification of artifacts, including hardware and software components, where the authenticity of entities, evidence, policy, and artifacts can be assured and the actions of entities can be guaranteed to be authorized, non-repudiable, immutable, and auditable. The proposed SCIM will be an industry standard specification, easing the path for uniform data flow across globally distributed supply chains.

SCIM aligns with an iterative approach to developing and implementing supply chain integrity requirements, allowing for enhancements over time based on evolving threat models and practices. A phased roll out of requirements promotes clarity for supplier planning and engineering and minimize disruptions.

Note: SCIM describes principles and a proposed model and system for conveying evidence. It does not address what evidence or information for attestation of conformity must be conveyed.

## Workflow

The following diagram depicts the flow of artifacts between entities in the Supply Chain Integrity Model. 

<p align="center"><img src="images/workflow.svg" width="450" align="middle"></p>

A Supplier creates an Artifact (a). An Attester creates Evidence (b) and submits to a Store for logging, query, and retrieval. The Supplier and Attester may be the same entity. A Policy Manager creates Policy (c) and submits to a Store where it is recorded and made available for query and retrieval. A User Agent receives an Artifact, retrieves Evidence and Policy, and verifies the Artifact (d). 

## Example Application

The diagram below shows an example application of SCIM to the Software Development Lifecycle (SDLC).

<p align="center"><img src="images/example.svg" width="900" align="middle"></p>

## Specifications

The table below maps proposed SCIM specifications to existing industry specifications.

SCIM | Existing
---- | --------
The SCIM-Evidence specification defines an extensible data model and exchange format for providing all types of evidence (bills of materials, build information, configuration settings, security assurances, certifications, vulnerabilities, end of life information) for all types of artifacts (hardware, software, services, machine learning models, etc.). | [SWID](https://nvd.nist.gov/products/swid), [SPDX](https://spdx.dev), [CycloneDX](https://cyclonedx.org), [in-toto](https://in-toto.io), [RATS](https://datatracker.ietf.org/doc/html/draft-ietf-rats-architecture-10), and others
The SCIM-Policy specification defines a data model and exchange format for providing policy for use in evaluating artifacts for a specified use. | [in-toto](https://in-toto.io), [RATS](https://datatracker.ietf.org/doc/html/draft-ietf-rats-architecture-10), and others
The SCIM-Store specification defines a rich, graph-aware storage API that allows publishing and subscribing to Evidence and Policy. | [DBOM](https://dbom-project.readthedocs.io/en/latest), [Grafeas](https://grafeas.io), [RATS](https://datatracker.ietf.org/doc/html/draft-ietf-rats-architecture-10), and others

## Roadmap

- Phase 1
  - Organizations use existing tools and specifications to begin implementing Section 4 requirements, including SBOMs.
  - SCIM community organized for the development of end-to-end standards.

- Phase 2
  - Organizations begin adopting SCIM specifications, which encompass and extend existing initiatives. 
  - SCIM specifications proposed to international standards bodies.

- Phase 3
  - SCIM specifications ratified by international standards bodies.
  - Widespread adoption of end-to-end model across globally distributed supply chains.

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
trademarks or logos is subject to and must follow 
[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
Any use of third-party trademarks or logos are subject to those third-party's policies.
