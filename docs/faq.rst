FAQ
========

Why shall I use WordLift? 
_____________

The purpose of using WordLift is to (1) categorize your content, (2) help people find content of interest to them, and (3) help WordLift describe your contents in *machine-readable* format so that other computers can re-use it. 

Why shall I publish my contents as Linked Data?
_____________

Richer metadata helps making content discoverable, searchable, and provides new means to reaching your audience.
Organising web contents around concepts or entities rather than traditional web pages helps improve navigation, content re-use, content re-purposing and search engine rankings.

Having content aggregations based on semantic annotations that use unambiguous Linked Data identifiers creates a richer navigation bringing the user experience to new levels of engagement. 

Who is using Linked Data today in the Media Industry?
_____________
Companies like BBC, Financial Times, New York Times, Washington Post, Reuters and Associated Press are investing in dynamic semantic publishing and use linked open data to organise their news portals and applications.

What is content enrichment? 
_____________

Content enrichment is a processes used to refine and improve textual content by embedding structured data (*metadata*) on web pages. This *metadata* is made available to search engines and other data consumers. 

What entity types are supported and how they map to Schema.org? 
_____________
*Thing*, *Person*, *Place*, *Event*, *Organization*, *LocalBusiness* and *Creative Work* are the supported types. 
Review the `Edit Entity page <edit-entity.html#entity-types-and-properties-table>`_ for more information.   

When should I create a new entity? 
_____________

You should create a new entity when this is directly relevant to the content you're writing and doesn't already exist. When an entity is properly recognised by WordLift you shall edit this entity rather then creating a new one. 

You can add as many entity as you like.

What are the guidelines for creating new entities to annotate a blog post or a page?
_____________

A basic guideline for adding a new entity is: 

	"*people should create entities that a librarian would plausibly use to classify the content as if it was a book.*"

The purpose of using WordLift is to (1) categorize your content, (2) help people find content of interest to them, and (3) help WordLift describe your contents in *machine-readable* format so that other computers can re-use it. 

In some cases key concepts that are important for (1), (2) and (3) are not automatically detected by WordLift and need to be taught. To teach WordLift new concepts a new entity shall be created.

.. note::

	When entities already exist we shall always avoid creating a new entity.

People should add entities that are accurate and directly relevant to the content they're writing, making it more likely that the content is seen by people who would be interested in it. 

A topic is directly relevant if the blog post (or page) is about the entity. If an article is not enriched with the main entity(ies) that it is about, people should add those entities.

Excessively broad entities should not be added to content. 

Content should not be overloaded with entities to increase its distribution online. As a general guideline, 8–16 entities should be adequate for most blog posts (based on the lenght of the article). If an article has too many entities it may be that some of the entities could be replaced with a single broader entity.

All entities shall be matched to the proper language of the content. 

What factors determine the rating of an entity?
_____________

The entity rating in WordLift takes under account the following factors:

- Every entity should be linked to one or more related posts. 
- Every entity should have its own description. 
- Every entity should link to other entities - when we select other entities to enrich the description of an entity we create a relationships in the site's `knowledge graph <key-concepts.html#knowledge-graph>`_.
- Entities, just like any post in WordPress, can be kept as draft. Only when we publish them they become available in the analysis and we can use them to classify our contents.
- Entities shall have a feautured image. When we add a featured image to an entity we’re adding the `schema-org:image` attribute to the entity.
- Every entity (unless we’re creating something completely new) should be interlinked with the same entity on at least one other dataset. This is called data interlinking and can be done by adding a link to the equivalent entity using the `sameAs` attribute.
- Every entity has a type (i.e. Person, Place, Organization, …) and every type has its own set of properties. When we complete all the properties of an entity we increase the entity visibility and usefulness.  

When should I link one entity to another? 
_____________

By running the analysis on the property description text of an entity I can *link* it with other entities. WordLift will store these relationships between one entity and other entities in the `graph <key-concepts.html#knowledge-graph>`_ using the Dublin Core property ``dct:related``. This information will be used to suggest new connections between the contents of your site. Though is not mandatory creating links among relevant entities will create more structure for your contents. I should always link entities that can help other users discover relevant contents (i.e. the entity *[Berners-Lee]* shall be linked to entity *[Web]* as the two concepts are strictly related).

Even if these connections between different entities might already exists in the openely available sources we use like DBpedia and Freebase by creating them inside our own `graph <key-concepts.html#knowledge-graph>`_ we will be able to leverage on. 

What are the languages supported by WordLift? 
_____________

WordLift currently supports the following languages: English, 中文 (Chinese), Español (Spanish), Русский (Russian), Português (Portuguese), Deutsch (German), Italiano (Italian), Nederlands (Dutch), Svenska (Swedish) and Dansk (Danish). 

.. note::
	WordLift supports one language at the time. The main language of the website can be configured from the WordLift settings. 
	Review the `configuration settings <getting-started.html#configuration>`_ for more information. 

What are the datasets WordLift uses for named entity recognition? 
_____________

WordLift by default uses DBpedia and Freebase to detect and link named entities. With a custom configuration, the content analysis services provided by `Redlink <http://www.redlink.co>`_ and available via our professional services, can use any RDF-based `graph <key-concepts.html#knowledge-graph>`_. It is also possible to use *multiple graphs* for named entity recognition and `dereferencing <key-concepts.html#dereferencing-http-uris>`_. 

What is a triple? 
_____________

A triple is a set of three elements: a subject, a predicate, and an object. Triples are linked together to form a `graph <key-concepts.html#knowledge-graph>`_ that is without hierarchy, is machine readable, and can be used to infer new facts. Triples in WordLift describe facts as metadata about an article or an entity. 
