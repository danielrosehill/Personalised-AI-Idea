# Personalised AI: A Potential Architecture

By: Daniel Rosehill.

Date: 28-Jan-25

The purpose of this Github repository, like many that I create, is to gather together a few thoughts and sketches for an idea that I have been working on for a couple of months as context storage and assistants and agents have all quickly advanced in maturity.

These notes bring together a couple of system components that I have been working on previously in an attempt to map out how a unified system for achieving this objective would function. 

Large language models develop their capabilities and a working knowledge of the world through exposure to training data. The selection of this training data is hugely influential upon the functionality of the ultimate model created. Therefore, determinations are required in training data selection. 

Even domain specific training data, however, is not personalized. To state the obvious, nobody wants details like their bank balance to be in the public domain. However, we have seen that when even small amounts of personalized contextual data are exposed to large language models, the results in terms of more personalized and relevant inference can be dramatic. 

RAG has quickly emerged as the normative mechanism to make the injection of this contextual data work. Using embedding models, files are converted into numeric representations and stored in specialized databases optimized for access by models. 

In its most simple implementation, this can take the form of allowing the user to upload a single file into a vector database, which can then be provided to a model or an assistant. The user might upload their resume, which gets converted into chunks, and then that gets embedded into a vector store to which an agent providing personalized career advice is connected. 

At scale, this process can happen dynamically. Rather than requiring that users manually upload files, a data store that is being continuously populated, like an S3 bucket or a Google Drive, is connected to the vector database through a RAG pipeline. This process has created enormous excitement for the use cases of RAG in business workflows such as internal tool development. A support team can be provided with a model which has access to the company's JIRA or Confluence. In this manner the latest internal information is always available to the agent and in turn the users. 




## Use Case Statement

## Author

Daniel Rosehill  
(public at danielrosehill dot com)

## Licensing

This repository is licensed under CC-BY-4.0 (Attribution 4.0 International) 
[License](https://creativecommons.org/licenses/by/4.0/)

### Summary of the License
The Creative Commons Attribution 4.0 International (CC BY 4.0) license allows others to:
- **Share**: Copy and redistribute the material in any medium or format.
- **Adapt**: Remix, transform, and build upon the material for any purpose, even commercially.

The licensor cannot revoke these freedoms as long as you follow the license terms.

#### License Terms
- **Attribution**: You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.
- **No additional restrictions**: You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.

For the full legal code, please visit the [Creative Commons website](https://creativecommons.org/licenses/by/4.0/legalcode).