This project is developed and presented during the [AI4CULTURE Hackathon](https://ai4culture.eu/) on 12-20 February 2025 at [KU Leuven](https://www.kuleuven.be/english/kuleuven/index.html), Belgium by the team ArcAIvision ([Sercan Kıyak](https://www.linkedin.com/in/sercankiyak/?originalSubdomain=be), [Elçin İstif İnci](www.linkedin.com/in/elcin-istifinci) and [Knar Ohanjanyan](https://www.linkedin.com/in/knar-ohanjanyan/?originalSubdomain=nl)).
Migration brings different stories, memories not just in the luggages and minds but also in the images. We, as three migration/media studies researchers, also together with our migration backgrounds, aimed to see which themes images hold within themselves. 

We chose to dive deeper into the Sound and Vision dataset from [The Netherlands Institute for Sound and Vision (NISV)](https://www.beeldengeluid.nl/en) to extract most common patterns in the migration-related videos that were not visible before in the collections. In such a large dataset it is difficult to investigate collective meanings and interpret results at a first glance. We therefore finetuned the data to see most common images related to migration. Our proposal can also be utilized beyond the topic of migration to investigate other connections and subjects in various video data.

We first worked on 30 samples (tagged with migration) to test whether our model could work. After obtaining the expected results, we expanded our sample to the entire dataset which did not have a tag. We grouped the images derived from the 30 samples.

We worked on a dataset consisting of 6421 videos retrieved from the Europeana API. After retrieving, we first clustered the videos based on their 
o	Description (en or nl)
o	Original URL
o	Europeana URL
o	Subject (these are labels attached to the videos) (en)
o	Location (en)
o	Date

We employed [BERTtopic](https://maartengr.github.io/BERTopic/getting_started/multimodal/multimodal.html), SentenceTransformer, pandas, VisualRepresentation and BeautifulSoup packages on Python.

We run the BERTopic multimodal clustering algorithm to find images that are similar to each other, the idea is to use these clustered images to find relevant film parts so that we can make a trailer or a short movie related to migration. 
o	We first did an image object extraction to find what are the objects in these extracted images. 
o	Then Bertopic clusters these images (we could also use the text data that we used before at this step but we feel it is not a good idea. The text data belongs to videos not images, we hope that by semantic associations between images we could capture more interesting and new connections).

![image](https://github.com/user-attachments/assets/8ea476f1-aa99-475c-b88f-1bbbfe94402e)


The clustered images and their minute and second information would then be used to create the film.


