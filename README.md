This project is developed and presented during the AI4CULTURE Hackathon on 12-20 February 2025 at KU Leuven, Belgium by the team ArcAIVision (@sercankiyak, @elcini and Knar Ohanjanyan, Elçin Istif Inci).
Migration brings different stories, memories, images not just in the mind and luggage but also in the atmosphere. We, as three migration/media studies researchers, also together with our migration backgrounds, aimed to see which themes images hold within themselves. 
We chose to dive deeper into the Sound and Vision dataset from The Netherlands Institute for Sound and Vision (NISV) to extract most common patterns in the migration-related videos that were not visible before in the collections. In such a large dataset it is difficult to investigate collective meanings and interpret results at a first glance. We therefore finetuned the data to see most common images related to migration. Our proposal can also be utilized beyond the topic of migration to investigate other connections and subjects in various video data.
We first worked on 30 samples (tagged with migration) to test whether our model could work. After obtaining the expected results, we expanded our sample to the entire dataset which did not have a tag. We grouped the images derived from the 30 samples
We worked on a dataset consisting of 6421 videos retrieved from the Europeana API. After retrieving, we first clustered the videos based on their 
o	Description (en or nl)
o	Original URL
o	Europeana URL
o	Subject (these are labels attached to the videos) (en)
o	Location (en)
o	Date

We employed BERTtopic, SentenceTransformer, pandas, VisualRepresentation and BeautifulSoup packages on Python.
