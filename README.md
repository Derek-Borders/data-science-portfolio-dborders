# data-science-portfolio-dborders

## Course Description  
*(Course Catalog, 2021-2022)*  
Data Science is the science of learning from data in order to gain useful predictions and insights.  
The course provides an overview of the wide area of data science, with a particular focus on the tools required to store, clean, manipulate, visualize, model, and ultimately extract information from various sources of data.  
Topics include the analytics life cycle, data integration and modeling in R/Python, relational databases and SQL, text processing and sentiment analysis, and data visualization.  
Emphasis is placed on reproducible research, code sharing, version control, and communicating results to a non-technical audience.  
(3 hours discussion)

## Potential Domains of Interest  
### 1. Natural Language Processing  
   This topic is the reason I first became interested in data science. I think this is the area with the greatest potential for near term, large scale economic impact as many forms of knowledge work can potentially be automated with tools we could build today or within a handful of years.  

   Presently, I am especially interested in improving computer recognition of common phrases, idioms, specialized jargon and slang as linguistic units. I am constantly noticing that spellcheck and automated assistants are very bad at (a) recognizing jargon I've used repeatedly, (b) correctly recognizing typos that involve unintended spaces, and (c) catching idioms and phrase errors that are clearly mistakes but that technically don't constitute spelling or grammar errors. I suspect there would be a lot of overlap in the solutions to (b) and (c), and that a solution for (a) might be a fairly straightforward data-mining operation that just hasn't been undertaken yet.  

### 2. Computer Vision / Procedural Generation
I am fascinated by a lot of the work in computer vision and procedural generation. I am most specifically interested in mapping and things like photogrammetry. Automation is also a very hot topic, of course, but I find myself thinking about turning pictures and videos into simulations more than autonomous vehicles.  

I love the idea of being able to recreate events and locations from old footage. I see procedural generation as a way to fill in the inevitable gaps in information needed to construct events and environments from limited information. This would certainly have applications in a number of industries, but I am most interested in the recreational possibilities. How great would it be to throw on a VR headset and explore crystal caves, senotes, ancient ruins, or even Middle Earth or Hoth. The demand can't support recreating every interesting location; it may never get there. But what if we could feed a scene from a movie into a program and it could reproduce the setting and extend it beyond the limits of the scene? What if we could step into some of our favorite scenes and watch them play out like we are right there in the middle of it all? 

I would also like to combine procedural generation with NLP to bring verbal descriptions of people, places, and events to life in a simulation. Again, this could be useful for various industries, but I mostly think about exploring books by just feeding a program the text and letting it build the world, characters and eventually even the events. 

I feel like we could come close to building a well described world or character with existing research projects today. I think reconstructing events is very nearly within reach as well. 

If such a tool existed, I could even see writers of all genres testing their descriptions against it to check that they are conveying the images they want to convey. Teams working on films and games could use such a thing to get a massive head start on developing the worlds they build by feeding such a thing more and more detailed descriptions of characters and settings.

Perhaps we could even port a classic game into a reasonable modern recreation with a video of somebody playing a level, or the text and images of an old guide book. Or maybe reskin the mechanics of one game with themes, settings and characters of a different game, or even a book or movie. (Let's not focus on the IP implications.)

### 3. Operational Analytics  
Aside from futuristic, cutting edge stuff I expect to be mostly beyond the scope of what I will see in undergrad courses, I am always interested in leveraging analytics for practical purpoases. I believe any size of business in any industry can benefit from working smarter. Application of the principles of data science (including traditional analytics) can help businesses optimize resource utilization, reduce costs, detect fraud, predict needs, identify bottlenecks, etc. Solutions can take the form of recommendation engines or price and/or inventory adjustment algorithms, or a myriad of other useful things.  

### 4. Data Visualization  
I love a nice data visualization. Something clean, clear, and aesthetically pleasing. I especially enjoy a nice report document full of such visualizations arranged to perfectly compliment the accompanying narrative explanation of whatever the report is about. I don't know that this constitutes a domain in and of itself. I think it is potentially relevant in a number of different domains.

## Data Science Questions  
### Question 1: Jargon
Given a domain (*ie* an industry or topic of interest) and an accompanying body of releveant text, can a tool be implemented to extract jargon and populate a specialized wordlist and export the list in a form that can be easily added to common spelling and grammar correction applications.  

#### Relevant Information  
I suspect the most useful information in implementing a solution here would be a body of text relevant to the topic in question. Presumably, some topics might benefit from varying types of relevant text, to account for jargon that tends to be more casual or more professional, for example. Others might be effectively solved by scraping the text from a relevant set of wiki articles or a subreddit dedicated to the topic in question. Still others may already have available wordlists or formal reference material that simply need to be converted into a useful format.  

#### Potential Data Source  

One topic that some user might like to have autocorrect leave them alone about might be names of medications. The FDA, CDC and other companies and agencies may have a comprehensive list of approved medications that could be scraped to generate a wordlist. This might be a sub-optimal source though.  

With a quick internet search, sites listing medications, such as [rxlist.com](https://www.rxlist.com/drugs/alpha_a.htm) can be found. A list of all words on such a site might adequate for the use case in question. In fact, this might be too comprehensive of a list. Perhaps a list of the most commonly prescribed medications and a similar list of the most popular over-the-counter medications would generate a smaller, more relevant wordlist. Another site, [ClinCalc.com](https://clincalc.com/DrugStats/) maintains a drug database that could potentially be queried directly with a specific scope in mind. The site also has several lists generated and available without interacting with the database directly, such as the *Top 200 Drugs of 2021* at the link above.

##### Data Set Features  
None of these are a proper data set, though one may be available. However, any of these resources could be converted into a list of unique words or a table of words and occurences. Occurrences would be less relevant for a list than for a body of regular text.

##### Potentially Useful Missing Features
For the narrowest version of the question at hand, lists of words may not be missing any useful features. 

However, the scope might be broadened to include definitions for words in these lists, or even other relevant data, if a solution were implemented as a plugin or independent application, rather than a list to add to existing dictionaries. If the scope of the question were so broadened, a more sophisticated model would need to be used, but the lists in the resources referenced are links which likely contain the additional information in question. 

##### Alternative Examples  
- A wordlist for Pokemon and their moves, types, etc. might be generated from the dedicated fan wiki site [Bulbapedia](https://bulbapedia.bulbagarden.net/wiki/Main_Page)  
- Similar wordlists might be generated for any of the many TV shows, movies, games, etc. with a section on [Fandom](https://www.fandom.com/).
- A wordlist for a particular course or an entire discipline (eg programming) might be generated from a relevant online textbook or tutorial site like [W3Schools](https://www.w3schools.com/).
