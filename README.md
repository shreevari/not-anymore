# not-anymore

### About
This is browser plug-in that filters out most important clauses from any list of Terms & Conditions(T&Cs) and also summarizes and visualizes results.

### Aim
- It aims to empower web users to make informed decisions online by knowing the tradeoffs mentioned in the Terms of Service.
- The main objective is to eduate the users about what bounds they have agreed to abide by and how their data is being managed by a service.

### How does it work?
#### Scraping Terms & Conditions / Terms of Service document : 
- JavaScript and Python are used to scrape the docuement from the website.
#### Filtering Important Terms : 
##### Dataset creation
- The dataset is created with contribution from the community via a website (inspired by the [Common Voice](https://voice.mozilla.org/) project)
- The dataset is compiled to a suitable format for use by anyone.
- This dataset will be open source too.
##### Machine Learning model - Training
- A Machine Learning model is trained with a suitable data-set built by the community.
- Bigger and more relevant the data-set, better the Classifier.
- More training = Accurate filtering.
##### Filtering
- User clicks on the extension icon
- Extension scrapes out the T&C document and feeds it to the trained model.
- The Classifier system picks out a few clauses that require the user's attention the most.
- The resulting few important clauses are displayed in a pop-up.
#### Summarizing :
##### Natural Language processing engine
- An NLP engine is trained with the help of existing datasets.
- The engine then summarizes the sections under the document.
- The Summarized content is made available in the form of an API.
##### Visualization
- The summarized data is visualized with the help of flow diagrams and associativity diagrams.

### What browsers will it be available for
- Currently, it will be developed as a firefox add-on.
- Chrome extension to follow quickly as we plan to use the WebExtensions standard.
