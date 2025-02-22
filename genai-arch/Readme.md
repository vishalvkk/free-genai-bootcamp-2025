# GenAI Arch Doc.

## Functional Requirements

The company (we) want to use their own infrastructure.
We want the technologies that do not have a vendor lock-in.
The technologies should be reasonably simple and powerful, to be oparated within permises and can be moved in, for example, cloud.
The data privacy is as essential as business logic.

They are starting with Manchester Urban areas where they expect users with niche requirements. They expect 1000 students at peak time and 200 generally. They want students to invest an AI PCs which can cost 10-45K GBP.

## Assumptions

We are assuming that the Open-source LLMs that we choose will be powerful enough to run on hardware with an investment of 10-15K.
We're going to host the application in Kubernetes cluster on cloud and we should be able to scale to the demand.
We expect APIs to provide interface of LLM systems we are going to host.
We expect that there are max 1000 students at peak times. Zero at least busy times.


## Data Strategy

Original work, plagiarism and copyrighted materials should be avoided.
Human Teachers are to supply high quality materials that can be stored in Vector DBs.
RAG to be implemented.
LLMs' knowledge can be enhanced on fly with internet search.
Unauthorised access to DBs should be protected.

## Considerations

We're considering using IBM Granite because its a truley open-source model with training data that is traceable so we can avoid any copyright issues and we are able to know what is going on in the model.

[IBM Granite](https://huggingface.co/ibm-granite)

We're considering meta-llama/Llama-3.2-11B-Vision-Instruct because it can 'see' data. The Llama 3.2-Vision instruction-tuned models are optimized for visual recognition, image reasoning, captioning, and answering general questions about an image. Llama 3.2-Vision is built on top of Llama 3.1 text-only model.


[Llama-3.2-11B](https://huggingface.co/meta-llama/Llama-3.2-11B-Vision-Instruct)