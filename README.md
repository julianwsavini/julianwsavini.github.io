# About Me

I am a detail-oriented, adaptable, ambitious student seeking employment in data science, UI/UX design, and product management. I am skilled in designing solutions, building applications, and supporting others in developing technical skills.

I recently worked as a data scientist for the Instiute for Experiential AI at the Roux Institute, where I created annotation guidelines and calculated statistics for RLHF in LLMs, improving data and pipeline performance. I have also modified DeepEval's faithfulness metric code to evaluate faithfulness in RAG systems, enhancing model evaluation accuracy. I am building a 1B parameter LLM from scratch, collaborating on model design, training, and optimization.

I am motivated to continue learning, honing my skills, and solving problems with technology. My strengths include quick mastery of new programming tools, collaboration across teams, and ability to evaluate and focus on end-user needs when designing interfaces.

As I explore professional roles, I am seeking opportunities to apply my technical skills while connecting with end-users to develop intuitive, user-friendly applications. Please feel free to contact me to learn more about my background and skillset.

# Projects

## Faithfulness for Instruction Giving
### Project Overview
During my data scientist co-op for the AI Solutions Hub at the Roux, I was tasked with working on a RAG project for Evity. Evity is a healthtech company focused on leveraging world class health research with AI to enable all people to live longer, healthier lives. The AI Solutions Hub developed a RAG (Retrieval Augmented Generation) model, which utilized medical papers to generate exercise regimines for customers, given their health conditions. I was specifically pulled in the project to lead RAG evaluation, specifically measuring faithfulness (which measures how well the outputs align with the medical papers).

### Initial Research/Implementaton
Originally, I researched multiple pre-existing evaluation frameworks, by reading 15+ papers on RAG evaluation, and viewing the frameworks' documentation. I ultimately decided to use DeepEval, for a multitude of reasons:
a) DeepEval compares statements from the RAG output (called "claims") to each statement from the relevant medical papers (called "truths"). This allows for more transparency, as I could see the assessment between each claim-truth pair.
b) DeepEval labels each claim-truth pair as either "supported", "not supported", or "no evidence". This third option prevents the model from being forced to pick between two options.
c) DeepEval is compatible with AWS Bedrock prompting methods. Other popular evaluation frameworks, such as RAGAS, are dependent on an OpenAI API.

However, after reviewing the outputs, we confirmed that DeepEval was not effective in evaluating faithfulness for our RAG model. There were three primary issues that lied in DeepEval's framework:
a) DeepEval ensures the generated truths are consistent with the LLM's pretrained world knowledge. This fact checking is not needed, and it strictly contradicts the premise that faithfulness measures how well the RAG adheres to the retreival context, regardless if the information is actually real or not.
b) 
c) compare the claims to the truths, as the framework could not compare imperative sentences from the RAG output, to the declarative sentences from the medical papers. Therefore, I got the opportunity to make my own evaluation framework, to properly evaluate faithfulness for the Evity RAG model.

## Recipe Recommendation System (Group Project)
For DS4300: Large Scale Information and Retrieval, we were tasked with using one or more NoSQL databases for our project. 

We established a goal of using a graph network to construct a recommendation system. I was responsible for design of the graph network and construction of the user interface. I drafted the graph network on paper, to be reviewed by the rest of my group. I then constructed the website using Python Flask, HTML, and CSS. At that point, my frontend engineering skills were still in their infancy, but it was great to have a frontend for a data project!

### Skills I developed:
- Graph Database Design
- Use of Python Flask
- Collaboration

<img src="https://github.com/julianwsavini/julianwsavini.github.io/assets/93225744/be9a18c4-7668-4dce-8f44-f7162d6b54a3"/>

Click [here](https://drive.google.com/file/d/1TiQC1zzqniXXINrGcj9z7QzKvLYAtVs-/view) to see the recommendation system in action!


## Data Visualization (Group Project) - [BlueBike Traffic/Accident Analysis](https://github.com/julianwsavini/BlueBikes_Visualization_Final_Project)
We were tasked with creating data visualizations to be used by a designated stakeholder. We designed an interactive graph for the team at BlueBikes that is responsible for establishing station locations. Our visualizations used bike accident data paired with station data, to hopefully increase safety for BlueBikes customers. The first graph is a heat map of bike accidents with points where stations are located. Hovering over the points shows the in- and out-flow of each station. If you switch modes, you can drag your mouse over the left graph to see where accidents occur (street versus intersection). This data can be used by BlueBikes when determining station locations farther from hazardous areas.

### What I contributed:
Once my group had created the heatmap, I was responsible for creating the bar and pie charts, as well as for linking these charts to the heat map such that they were interactive. This involved creating tooltips, brushing and linking, and making possible the hovering over of elements to regenerate new graphs. I played a large part in the design process, as I assessed who our stakeholders were, and determined which visualizations would be most useful in their decision making, regarding safe placement of BlueBikes stations.

### Tech Stack:
- HTML
- CSS
- Javascript (d3 library)

### Skills I developed:
- Creation of interactive visualizations using Javascript's d3 library
- Design Thinking
- Collaboration

Check out site here: [BlueBikes Visualization](https://ds4200-s23-class.github.io/project-julian-jake-david-aneek/)


## Machine Learning - [News Classifier](https://github.com/julianwsavini/news_classification)
Although this project was completed during only my second year of programming, I stretched my skillset and decided to use use Natural Language Processing and Machine Learning to determine if a news article contains false information.

This was a group project, and I was responsible for constructing the machine learning models. Other group members did not have Python experience, and we wanted for each member to play to their strengths.  Therefore, as others did research and created the project proposals, posters, and slides, I was excited to handle machine learning tasks. I utilized K-Nearest Neighbors, Gaussian NB, and Random Forest models to train my data, with the best model achieving 89.2% accuracy.

### Skills I developed:
- Natural Language Processing Data Cleaning Methods (Count and Term Frequency-Inverse Document Frequency Vectorizers)
- Hyperparameter Testing
- Utilization of many functions within the sklearn library

  
## UI/UX Design (Co-Op) - ISS Group - [See UI Here](https://github.com/julianwsavini/Co-Op-Project)
I was tasked with the redesign of one of ISS Group's frontend products, iPurchase. This was done using Material Design Bootstrap. There are loads of features within this UI, such as dynamic field labels, tabs which transform into an accordion when the screen size is small, and tables that change layout depending upon screen size. It was fantastic to be deeply involved in creating their new UI, and I appreciate that the group involved in review and decision making was never content with whichever incarnation of the product was in front of them. We knew we could always make the system better, so iPurchase underwent many, many design iterations. It was a fantastic first co-op experience, and I'm excited to see what I'll be doing next!

Until May, I am working part-time for ISS Group, conducting UX research with our clientele, hoping to gain more insight as to what works with our frontend, and what does not. In addition, I will work on rebuilding the frontend using ReactJS.

Tech Stack:
- HTML
- CSS (MDBootstrap)
- Javascript

<img src="https://github.com/julianwsavini/julianwsavini.github.io/assets/93225744/a285bfc4-d173-47a9-b01d-f63eac242d0e"/>

# Contact
Email: savini.j@northeastern.edu

Some of the roles I am interested in:
- Data Science
- Data Analytics
- Data Visualization
- Data Engineering
- Product Management
- UI/UX Design
