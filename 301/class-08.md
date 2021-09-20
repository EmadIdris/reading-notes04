# Readings: APIs

+ ## It stands for **Representational State Transfer**.

+ ## REST APIs are designed around a **resource**.

> Resource identification refers to the unambiguous reporting of research resources such as genes, organisms, tools, and reagents (such as antibodies). These resources should be reported within publications with enough information that reviewers and subsequent researchers can identify the exact strain or reagent used. Preferably, authors should provide the full, descriptive name of the resource, its source and a unique identifier. Doing so allows for:

+ Better evaluation of the methods and interpretation of results
+ Reproducibility of the research
+ Machine readability and potential text mining applications

> Many reporting standards will include guidance on how to identify such resources. This page provides further information and sources for unambiguous identifiers.

[Examble](https://saylordotorg.github.io/text_building-strategy-and-performance/s03-02-identifying-resources.html)

***
+ `GET`
+ `POST`
+ `PUT`
+ `PATCH`
+ `DELETE`

***

> A Uniform Resource Identifier (URI) is a unique sequence of characters that identifies a logical or physical resource used by web technologies. URIs may be used to identify anything, including real-world objects, such as people and places, concepts, or information resources such as web pages and books. Some URIs provide a means of locating and retrieving information resources on a network (either on the Internet or on another private network, such as a computer filesystem or an Intranet)

[Examble](https://blog.hubspot.com/website/application-programming-interface-api)

***
### Why chatty API is bad?

+ Reason why chatty APIs are considered poor quality is because requiring multiple network calls will slow down an application. This is because each call contains data overhead (i.e. sender information, headers, authentication) which will slow down an application as well as network latency per each request.

***

+ ## It *returns* an **HTTP status code 200 (OK)**.

+ ## It *returns* a **404 (Not Found)**.

+ ## It *returns* an **HTTP status code 201 (Created)**.

+ ## It *returns* an **HTTP status code 204 (No Content)**.
