### Bibliometrics

The overall goal of science is to gather statements about reality through observation and experimentation, to predict events based on natural laws, i.e. to produce new knowledge. Based on this knowledge, new technologies and applications can be developed. New scientific knowledge is mainly communicated through the publication of documents, such as articles in scientific journals or, in the case of immediately applicable knowledge, as patent specifications.

#### Scientific publications

A scientific publication (i.e., a "paper" or an "article" in short) disseminates empirical and theoretical findings in a more or less standardized form. Scientific publications are currently divided into the following types:

Scientific articles published in journals
Conference presentations published in conference proceedings
Books, which are completely written by one or more authors
Patent specifications
Technical reports and working papers
Other types, such as government reports
Articles can again be divided into different types:
Original articles, case reports, technical notes, image essays, reviews, commentaries, editorials, and others. As part of an academic publishing process, publications are typically peer-reviewed by subject matter experts to ensure quality, relevance, integrity, and readability.

Articles contain the scientific content as well as bibliographic information that helps to categorize and find the former.  

The following figure shows an example of a journal article with bibliographic information (e.g., article title, name of the journal, information about authors, license) and its content ("full text").  Articles typically contain an abstract (a short summary) and references, i.e., a list of publications that have been cited by the paper and describe contexts, for example, whether the paper is based on findings of other papers or whether it confirms, extends, mentions, or disputes them.

References appear at the end of a publication, while citations (sometimes also called in-text citations or cites) appear in the content of a publication and point readers to the references. Citations can appear in an article in two ways: parenthetically (such as "Meier, 2020; Huang, 2014; McClintock, 2011") and narratively (e.g., "Meier (2020), Huang (2014), and McClintock (2011) extended the wood-color theory"). Furthermore, citations can be specified either as numbers in ascending order or with author name and year of publication, as in the example above. The format normally is specified by the publisher. For example, Springer typically uses numbering in the computer science field.

#### Analysis of scientific publications

Scientific publications can be analyzed on the basis of their bibliometric data, including the analysis of references. The actual content of the article can also be analyzed using methods of data mining and natural language processing.

The analysis of publication metadata is called bibliometric analysis. In addition to familiar descriptive statistics, which include metrics such as the h- and i10-index and the so-called journal impact factor (JIF), these also comprise analyses of networks, which consist of interlinked bibliometric entities. Bibliometric entities, in turn, are entities such as an academic publication, an author, a journal, an institution, a country, a keyword, and so on. By applying algorithms known from graph theory, various types of so-called communities can be computed and predicted. These include, among others:

Knowledge Bases: groups of scientific publications in a research area on which the field is based.
Research Fronts: groups of scientific publications in a research area that address similar (unsolved) research problems.
Classics: scientific publications that are outstanding and have a major impact on a research area.
Field Players: authors, organizations, or countries that make a significant contribution to a research area.

##### Bibliometric Networks

Scientific publications typically contain references to other publications or even source code, for example, and thus describe relationships between these entities. Thus, scientific publications and other bibliometric entities, such as authors, can be represented and analyzed as a mathematical graph, which are called "bibliometric networks" in the following.

Bibliometric networks describe affiliations (memberships) or similarities of bibliometric entities and are used to find groups of similar entities and relations to other entities or groups. In 1965, Price investigated the citation behavior of journal articles and started the field of bibliometric networks by depicting a network of journal articles. A minimalistic example of an article network is shown below.  

Price's network shows journal articles as nodes and references between articles as directed edges, i.e., there is an edge from node one to node two if node one cites node two. In the case of the network shown, both article one and two cite article three.

Based on the idea of Price, different types of bibliometric networks were developed. In general, two types exist: membership networks and similarity networks, where membership networks describe the affiliation (i.e., a relation) of bibliometric entities while similarity networks express similarities, i.e., with a similarity measure between bibliometric entities, such as "A is 40% similar to B based on a given metric".

##### Membership Networks

Mathematically, membership networks are represented by a weighted, directed graph whose nodes represent bibliometric entities of any type (see figure above). The most common are bipartite membership networks, which represent a bipartite graph, i.e., there are only two types of nodes in the graph, and nodes of the same type may not be directly connected.

Bipartite membership networks are named after their entity types, e.g., in an author-publication network, the nodes either depict an author or a publication while the edges represent an affiliation from an author to a publication or vise versa. An intuitive example of such an affiliation is that there is an edge in the graph from an author to a publication if the author wrote the publication. Price's network of journal articles can be seen as a special kind of affiliation network, where articles are the only entity type in the network.

##### Similarity Networks

The second type of bibliometric networks are similarity networks. From a mathematical viewpoint, similarity networks are weighted, undirected graphs. Every node of the graph represents an entity of the same type, e.g., all nodes represent authors. Nodes are connected by weighted, undirected edges, depicting the similarity between the connected nodes. These similarities are calculated by using a similarity measure expressing the similarity of two bibliometric entities.

Depending on the type of bibliometric entity, different similarity measures can be used. An example of a similarity measure for authors is co-authorship. Co-authorship between two authors is defined by the number of academic publications they have published together.

To measure publication similarity, co-citation and bibliographic coupling as well as lexical measures are commonly used. For example, two publications are co-cited if both publications are cited by a third publication, while two publications are bibliographically coupled if one or more citations from them are similar (see section below).

Similarity networks are named after the similarity measure used to compute the similarities, e.g., a co-authorship network is a network whose nodes represent authors and whose edges represent their similarity based on the co-authorship measure. Many similarity networks can be computed based on bipartite membership networks. Some types of similarity networks are presented below.

##### Author Networks

Any bibliometric network that contains authors represented as nodes is considered an author network. Thus, any membership network that contains authors and any similarity network based on a similarity measure between authors is considered an author network. Like any similarity network, author networks are computed based on a similarity measure that defines a similarity between two authors.

There are many possibilities for measuring author similarity.  For example, similarity between two authors can be measured by counting the number of conferences at which they were both present. A more common example of an author similarity measure is co-authorship. Again, co-authorship between two authors is defined by the number of academic publications they have published together. An example of a co-author network with its associated author-publication network is shown below.

On the left side of the figure above, the bipartite graph of the author-publication network is shown, with authors in gray and publications in orange. On the right side, the resulting co-authorship network is shown. Authors two and three are coupled by two publications they published together, while author one is coupled by only one publication with authors two and three. Author four is not coupled with any other author, having published only one publication on his own.

##### Publication Networks

Any bibliometric network that contains academic publications as nodes is considered a publication network. The corresponding membership network is the publication-citation network, which consists of nodes representing an academic publication.

A co-citation of two publications is given if both publications are cited by a third publication (see figure below), the two publications are then considered a knowledge base.

The counterpart to co-citation is bibliographic coupling, another similarity measure for academic publications. If one or more citations of two publications are similar, the two publications are considered bibliographically coupled (see figure above). Bibliographically coupled publications form a so-called research front. While knowledge bases describe sets of publications that may have been published for a longer period of time, research fronts may represent relationships between publications that have also been published recently.

Besides those two similarity measures, which are based on the citations of publications, lexical measures can be used to define the similarity of publications. Lexical measures compare the textual content of publications, as for example the title, keywords, abstract or full text. If two publications contain the same word, they are connected by this word. In information retrieval theory, term occurrences in documents can be described by a document-feature-matrix (DFM) whose entry yields a term frequency, i.e. how often a publication contains a specific word.

Lexical similarity measures pose a problem that needs to be addressed: simple counting of words (which is done when creating a DFM) favors those words that occur often within many publications, what may be counterproductive, as those words may not reflect an interesting similarity between publications. Intuitively, more meaningful are words, that occur often in only few publications.  To account for this problem the "term frequency inverse document frequency" measure (TF-IDF) can be used.

As seen, there are many types of bibliometric networks that can be used for diverse applications. One application is the computation and visualization of research fronts, i.e., groups of academic publications of a research field on which it is based. How this is achieved is outlined in the following section.

#### Visualization of Research Fronts

Researchers may be interested in obtaining an overview of current research fronts in their research area. These research fronts consist of academic publications that are linked by their citations and describe an emerging research field or topic, which in turn is formed by similar in content publications.

Bibliometric methods can be used to find these research fronts. The following section provides an example of how to find groups of academic publications that address similar research problems. Based on similarity networks of academic publications, groups/communities of publications (sometimes also called clusters) can be formed and visualized. Since a research field typically contains several thousand publications, visualizing the communities found is challenging.

An example of the visualization of such a network is shown below. It consists of 3000 academic publications, where each color represents a community calculated using the Louvain method. Each community is a candidate for a research front, e.g., it could represent an upcoming research topic. This technique can be used to identify research fronts that were previously unknown to the researcher.

#### Bibliometric Analysis Process

In order to perform bibliometric analyses, several steps must be performed. A simplified and general purpose process for bibliometric analyses is described below.

At the beginning of a bibliometric analysis, its objectives must be defined (1), i.e., what kind of results are expected, e.g., finding research fronts and bodies of knowledge. Next, a data set must be collected (2). To do this, one or more data sources must be selected. Commonly used bibliometric data providers are Web of Science (WOS), Scopus, Google Scholar, and Microsoft Academic. This step also includes the definition of queries that can be used to find a set of relevant publications in the respective databases.  Furthermore, the raw data must be exported from these databases and then preprocessed (3). This may consist of data cleaning, e.g., removing duplicates and incomplete records, enriching the dataset with data from additional information sources, and, if multiple data sources are used, merging the raw data. Based on the defined objectives of the bibliometric analysis to be performed, some bibliometric algorithms are selected and executed to calculate (4) and visualize (5) the results. Finally, the results have to be interpreted (6).  As in classical Knowledge Discovery in Databases (KDD process), it is possible and it may be necessary to adapt and re-execute a process step. For example, a search query may need to be adjusted to exclude unwanted search results that should not be part of the analysis.

AMBALYTICS aims to support and automate steps (2) to (6), so a user only has to define the target of his analysis and interpret found results. Thus, for example, a structured literature review (SLR) performed using the AMBALYTICS platform can be combined with bibliometric analyses to significantly reduce the execution time of an SLR while simultaneously considering a larger set of publications.

#### Limitations of Bibliometric Analyses

Bibliometric analyses, like any other method of calculation and interpretation, have a few limitations:

Hidden knowledge: Scientific findings are not always published as academic publications or even not published at all. Furthermore, qualitative findings, such as expert opinions, are not taken into account by the bibliometric analysis. Thus, those areas are better suited for the application of bibliometric analyses in which there is a lot of continuous scientific publication and subject databases with further structured information are available. This is the case, for example, for large parts of the academic medical field: in this field, scientific findings are published often and frequently in publicly accessible formats.

Dataset creation: Any bibliometric analysis is based on a dataset of bibliometric entities that must be obtained. Typically, bibliometric databases are queried and the results are extracted.  Thus, the query terms influence analysis results. These queries can be improved by helping users create them.

Data volumes: The more bibliometric entities to be analyzed, the larger the resulting similarity matrices. AMBALYTICS uses different technologies to be able to analyze even larger data sets quickly. Among other techniques, a distributed infrastructure is used.

Time delay: The data available in publication databases is a snapshot of academic knowledge that does not fully represent the current state of science, as it takes between 4-6 days and up to two years for research results to be published and listed in these databases. A combination of several bibliometric databases can achieve greater coverage and shorten the time to integration in searches. The evaluation of other data sources, such as social networks, can also shorten the time to integration.

Publish or perish: Because the number of publications and citations has some influence on the evaluation of authors and institutions, some co-authorships do not reflect actual collaboration. In addition, self-citations and citations in review publications may not be content-based. Here, for example, content-based methods or even the combination of different methods, as used also by AMBALYTICS, can calculate the actual influence more accurately.

#### Applications and Use Cases

Bibliometric analyses can be used for a whole range of use cases. For example, they are part of the methodology for evaluating research and influence the way university rankings are calculated or how individual institutes within research institutions are financially remunerated. Bibliometric indicators of productivity, impact, and collaboration among researchers, institutions, and countries, therefore, are used to evaluate research. Evaluation results can provide an unbiased, quantitative basis for decision-making, e.g., to justify decisions about funding for scientific projects.
Bibliometrics can also help discover the structure and dynamics of science itself, also known as science of science. Bibliometric concepts can be used to identify future developments in research fields or for technology foresight as trends and forecasts.
Finally, automated procedures such as bibliometric analyses as well as integrated platforms like AMBALYTICS can facilitate and accelerate the everyday life of people working in science, for example through contextualized searches, configurable visualizations, or even auxiliary functions such as the automatic transmission of found references to other tools used in this workflow (e.g., reference management software like Mendeley or Zotero).

