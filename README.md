# Star Wars Dataset
Hello there, young Jedi and seasoned Star Wars fans alike!

In a galaxy not so far away, a new data repository has emerged to deepen our understanding of the Star Wars universe.
I'm excited to announce the release of a special dataset containing information about the planets, characters, movies, and TV series from our beloved Star Wars universe: our **Holocron**.
This dataset is compiled from text pages on Wikipedia, since I couldn't get permission to use data from Wookieepedia.

<p align="center">
  <img src="assets/logo_2.png"/ alt="Star Wars logo">
</p>

## Dataset Introduction

### What’s in the Holocron?
This dataset is like a Holocron, packed with detailed knowledge about the galaxy far, far away. You’ll discover entries on various planets, iconic characters, and significant events from the movies and TV shows.

### Unveiling RAG (Retrieval-Augmented Generation)
For those unfamiliar with the term, RAG (Retrieval-Augmented Generation) is a powerful AI technique that combines the best of both worlds: the vast knowledge stored in a dataset and the generative capabilities of AI. In the context of our Star Wars dataset, RAG can be used to answer intricate questions, generate detailed character backstories, or even create immersive fan fiction that adheres closely to the established lore.

#### How RAG Works:
- Pose a Question: For example, "What is the story of the planet Mandalore?"
- Search the Holocron: The AI searches the dataset for relevant entries on Mandalore, including its political history, key events, and notable figures like Duchess Satine Kryze and Bo-Katan Kryze.
- Create a Holocron Entry: The AI combines the information to craft a detailed and accurate response.

*Example:* ``` Mandalore, a planet with a rich and tumultuous history, played a pivotal role during the Clone Wars. Known for its warrior culture, Mandalore was led by Duchess Satine Kryze, who advocated for pacifism. However, the planet was engulfed in conflict as various factions, including the Death Watch led by Pre Vizsla and later Darth Maul, sought control. Bo-Katan Kryze, a prominent warrior and sister to Duchess Satine, ultimately played a crucial role in liberating Mandalore from Maul’s grip, setting the stage for future battles and the eventual rise of the Mandalorian way under her leadership. ```

### The Force Behind the Dataset
This dataset is designed with flexibility in mind, enabling seamless updates in the future. Alongside the dataset, I've released the code used for its creation. This means that whenever new Star Wars content emerges, you can just run the code and you will be able to retrieve a new dataset containing all the latest information regarding the lore. If there is something I missed and that should be included in the dataset, feel free to improve the dataset.

### Joining Forces
I invite you to explore this dataset and perhaps contribute to its expansion. With every update, we enrich our collective understanding and appreciation of the Star Wars saga. Whether you're a data scientist, a programmer, or simply a Star Wars enthusiast, your contributions can help keep this repository as dynamic and expansive as the galaxy itself. I probably didn't cover all the possible cases and there might still be work to do. That's why this dataset needs you, young Padawan and Jedi Masters.
However, keep in mind that the dataset was originally thought for a RAG application. As not everyone owns a GPU, indexing too large sources of data may be infeasible. Keep that in mind, probably releasing different dataset sizes could be an option.

*May the Force be with you. Always.*

## How to run the code

#### If you want to use the dataset directly
Simply download and extract the dataset.zip file. You have already access to all the files contained in the dataset.

#### If you want to re-extract the files for updated information
I have created the file wiki_scrape.py with the goal of extracting all the information in the simplest possible way.

First of all, clone the repository from the terminal window:
```
git clone https://github.com/AlbertoFormaggio1/star_wars_unstructured_dataset.git
```

##### Environment configuration
To run this code you need very little configuration. From inside the virtual environment you are using (either venv or conda) install BeautifulSoup and Requests:
```
pip install requests
pip install beautifulsoup4
```

##### Run the code
Now we can extract our dataset by running the wiki_scrape.py script.
```
python wiki_scrape.py
```

That's it! You can now play with your freshly extracted dataset!

Have a safe journey in this dataset.
