# 2019 csvconf Notes
**Schedule:**
https://csvconf.com/speakers/

### schedule
---

10:30a
**The Time is now**
**Afua Bruce** 
Director of engineering, public interest, technology


Abstract:
Despite the tech world’s image of being fast-moving and constantly evolving, segments of those working in, or wanting to work in, tech are often told to wait. It’s no secret that the tech and data worlds do not reflect the nation’s diversity. And for those of us working in Civic Tech or Public Interest Technology, the struggle to secure long-term funding for projects or identify career paths is real. What if we shifted our mindset from “with a lot of time and a lot of work, we’ll figure it out,” to “let’s experiment and incite change today.” The time is now to tackle the question: as the data-driven community matures, how does it do so in a way that’s inclusive and sustainable?


Tech & innovation
tech innoation is an extended concept of innovation

lead for pub insterest tech program 
managing implementation projects that address social issues 
fundraising for core costs and op costs 
bulding partnerships with gov, non profits, communities
learning from and teaching others in the public interest tech space


Common struggles 
mission-driven wanting greater impact 
how do we atract people to do this work ? 

what do we mean bu inovation? 
what works for innovating on how we do the work to innovate
identify self, find funding, rely on models in other spaces 
contiuned progess, focus in 3 areas 
div, and inclustion, working models, funding 

diversity inclustion:
struggle with this idea 
tech ovreall lacks diverstiy 
difference between 
designming for and designing with 
including people at the table and inclusion talking to the people at the table 



working models:
fellowships 
consolidating analyzing and presentating data 
long-lasting community partnerships 
business ventures 

funding the work 
pholothranphic dollars, 
academic grants 
fisncal sponsors 
social enterprises 


what will we do in one of three catagories?  

diversity and inclusion 
working models 
funding the work 


what can we do differently , different ways to do buniness? 


---


11:00a

**Alexander Morley**	
**What's Next after Notebooks?**

Jane is a data scientist. Jane uses Jupyter notebooks as her working environment, and her presentation environment. These “computational essays” allow Jane to present her methods and her results to her colleagues at the same time. Jane is happy with this. But sometimes it’s difficult for Jane to share notebooks with her colleagues, and even harder for them to re-mix or re-use parts of the notebook, or to share their changes back to Jane. And sometimes Jane finds it hard to explain the flow of a particular notebook, or how different notebooks are tied together. There’s no provision for keeping things modular. First, I will discuss a few up-and-coming projects that are leveraging the power of new web technologies and faster browsers to solve all of fictional Jane’s problems, and more. Second, I will present a prototype for my own solution that is also web-based, and draws inspiration from some now-uncool graphical programming languages.



Essay or Choose your own adventure 
diff of sharing a nice story vs sharing the whole process

Q&A 



---




11:30a
**Bash <3's CSVs: Data Analysis on the cmdline**
**Nicholas Canzoneri**  Github

Your bash shell has a _lot_ utilities that can be used to help you analyze your data, often easier and faster than trying to import your data to an external tool. But these utilities can be hard to find and even harder to figure out the right options. I'll walkthrough a data set and show examples of the best utility to use in different situations. I'll go over common commands like `grep` and `cut`, more exotic commands like `comm` and `tr`, and dig up very useful options to a command you might have overlooked, like `sort -k`.

Bash - uses 235x tims faster 
multi gig range 

when is bash good to use 
line based data 
consistent structure, e.g. csv, server logs
not good for json or xml 

peeking at the data using:
`head` 
`tail`
`wc -l`
`grep` & `grep -v`

`cut -d ' ' -f1` chop up lines in a consistent manner 
`sort`
`sort -t ',' -k2,2 -k3,3nr  population.csv`
`sort -u`
`sort -k`

pipe commands 

**Bash working with multiple files:**
Join command

`paste -d or -s`

`seq 1,5` 

**comparing files** 
`comm` 
`comm -12 ohio_cities.csv missouru_cities.csv` 

**deal with cleanup**
`sed`
`tr` - translating 

**example**
Raw data from Census 
parsing data 
gettiing rid of data 
`cat` pipe `tail`
`cut -d`  - get fields you want
`sed`  - search and replace quotes
`sed` remvoe leading space  > save file

getting a word count
`cat, tr -d, tr -s, tr, tr, sort -u -c, sort -nr`

`jq` - command to work with JSON

examples on:
github.com/nickcanz/csvconf2019

learn to read the `man` pages to figure out how to do things 



---

#### 12:30 Keynote
**Kari L. Jordan

Imposter syndrome 
fundamental data skills for research 

what makes an expert- creating a comfortable environment for people to contribute to their work 

terminology: 
accessibility 
e.g. running workshops on a budget 

diverisety
differences engaged in the service of learning 


equity
creating access and participation in programs

equality vs equity -fairness access to the same opportunities 


inclusion 
engagement of diverse people and communities 


Verna Myers quote
diversity is being invited to the party.  Inclusion is being asked to dance


approaches to build confidece to work with data:

training for data skills averting the crisis 
importance of guidance instruction - need to teacdh people 

training the intended user base and how to measure them. 

reach diverse pop. through training 
how do we train people? 

empower people to work with more data 

### carpentries: inclusive pedagogy 
short impactful workshops 
Open sounrce contributions 
provide regional support communities 

foundational computational research data science skills 

evidence based teaching approaches 

### swc Pedagogy:
teaching practices 

Resilience and persistence when working with data 

approachs to build confidence to wokr with data 
short focused learning experiences 



caprentries is teaches a community of practice 


self ecfficacy indivd believe she is capable of taking action to achieve a certain goal 


4 pillars fo self efficacy: 
performance outcomes - 
vicarious experiences e.g. live coding 

vicatious experiences 
pracitce and receivce continuous feedback 
learning by watchign how other do things 

verbal persuasions - 
supportive people - help build self- effaccy 
mentoring groups in carpentries 
foster community building


physiological feedback - 
learning environemnts can create anxiety

participation a harassment free environment - code of conduct 
open and inclusie learning environments 


https://urlzs.com/M7XU

skills to address questions that are important to them 



situational task specific 


how to support learners - train the trainer 
support the community 

south east asia - instructors 
hard to build local community and capacity 





---


1:30p
**The n-of-many-ones:Fueling Community Science with Personal Data**
**Bastian Greshake Tzovaras**
As we are becoming more and more digitized, we are creating and collecting more personal data than ever before, offering unprecedented chances for research. This potential wealth of data for research comes practical problems such as: How to merge data streams? And how can people responsibly share their personal information? In this talk we will explore how to enable responsible personal data sharing by giving individuals granular sharing options and how this can enable community science. Furthermore, we will also see how we can scale up personal data exploration from the n-of-one to an n-of-many-ones, using a JupyterHub setup built right into a community science platform.


data sources - Google takeouts, twitter archives, genetic data 
continuous API integrations (fitbits, cont. glucose monitors, device usage data )
data storage standardized by data source - 

using OpensHuman account, use API in juptyer notebook 

participatory reserach 
e.g. connecting glucose monitor data - Dana Lewis Open Artificial Pancreas System 
#openAPS 
NightScout tech 

open data in data commons contributing to CGM data 


Qcycle and UC Berkeley 

individual centri personal dat sharing 

Governance building trust and community - 
how do you build trust in the community - community elected and board elected 


import own data 
explore and share data via notebooks 
share data with cool research projects 

research groups:
Berkeley Lab
OpenHUmans




Sponsors:
Google summer of code 






2:00p

**Social Data: Invading Privacy or Creating Better Cities?**
**Gala Camacho**

Urban designers have long heralded the value of the public realm in creating stronger communities. Yet, their processes and decisions are based around data that is far removed from the community, outdated and/or based on surveys and feedback forums which are generally attended by the same group of people and which can be overtaken by lobbyists. If we want to create cities that place people at the centre, it is essential that we find data about what makes neighbourhoods connected and wholesome, neighbourhoods which provide safe spaces for their community to engage. Social data (data from social media, crowdsourcing, mapping platforms, review apps, etc) can give us an opportunity to understand how people engage in their communities and interact with the places around them. It can be used to provide insights into the social health of local places and identify vulnerabilities, to feel the heartbeat of the neighbourhood. I will talk about what social data is, some of the challenges of getting it and collating it, the data's strengths and weaknesses, and how we are trying using it to make cities more socially connected.


City making:

surveys to collect data about the cities 

city makers trying to make clear the data they are collection but it is difficult 

social data:
has a geo spatial component link to physical place 
derivce drom digital sources 
place focus 
people's behaviors and life styles 


can we shift using people's privacy data towrds making better cities
getting data from social media 

there are strengths of social data 
scalable, oganically generated, reactive, live, world wide, verifiable, accessible for people 


---

2:30pm


**US Energy Data Liberation**
**Zane Selvans**

An alphabet soup of government agencies like FERC, EPA, EIA, PHMSA, MSHA and the ISOs and RTOs collect and publish terabytes of data about the US energy system. It includes operating costs and fuel consumption, hourly power output and GHG emissions, and the age and length of natural gas pipelines, the price of electricity every 5 minutes at thousands of nodes in the grid, coal production numbers and much much more. In theory all this data is public and freely available, but in practice it takes a lot of wrangling to make it usable for analysis. The result: it's packaged up by one or two platform monopolies that charge tens of thousands of dollars a year for easy access, excluding most non-corporate users. But for anyone interested in the ongoing transformation of our energy system and its climate impacts, this data is a treasure trove worth excavating. The Public Utility Data Liberation project (https://github.com/catalyst-cooperative/pudl) has been working for the last 2.5 years to liberate this data and make it freely accessible to activists, data journalists, and researchers working on US climate and energy policy. This talk will take a look at what the data is, where it comes from, why it's interesting, how we're processing it and making it available, and some of the challenges we're facing and opportunities we see ahead.



public utiliies commission

Catalyst - prject to use data 

souces of datas - 
organizations that run the grid. ISOs 
data sets give information about costs and data systems 



---


3:30pm

**Qualitative Research Using Open Source Tools**
**Beth Duckles & Vicky Steeves**

Qualitative research has long suffered from a lack of free tools for analysis, leaving no options for researchers without significant funds for software licenses. This presents significant challenges for equity. This panel discussion will explore the first two free/libre open source qualitative analysis tools out there: qcoder (R package) and Taguette (desktop application). Drawing from the diverse backgrounds of the presenters (social science, library & information science, software engineering), we will discuss what openness and extensibility means for qualitative research, and how the two tools we've built facilitate equitable, open sharing.



Why qualittive data methods? 
Answers questions that quantitative data studies cannot 


How QDA tools comparison:
NVIVO
MAXQDA
Atlas, TI
Qualcoder free
Qcoder(R) free
Taguette free


Why FLOSS QDA Tools 

Culture 
data privacy concerns both with own and open data 
open souce can be as secure 

education - GUIs taining adn easy setup 

technological

open initiativss in Qual
Past FLOSS QDA initiatives (defunct)

Rotterdam Exchange Format Initiative 

Qual needs more quitable access to software 

rOpenSci unconference - developed a prototype, still in dev. 

**Qcoder**
uses RSTudio and SHiny 

using codes books as examples 

github under ropenscilabs https://github.com/ropenscilabs/qcoder 
looking for collaborators 

**Taguette** - 
app.taguette.org 


multilingual tool, contribute to translation 


qual researchers need FLOSS apps trying to fix they gap. 



---


4:00pm 

How to Feed Your Robot: Building and Maintaining Open Machine Learning Datasets
Evan Tachovsky - rockerfeller foundation

While algorithms and computing power get all the press, the special sauce behind many recent machine learning breakthroughs are meticulously labeled training data. Developing and maintaining these data sets as public goods is both an art and a science. In this talk I'll present a new set of best practices gleaned from interview with ~20 data set builders, maintainers, and funders. Topics include: encouraging collaboration between rival data teams; finding and addressing ethical issues with crowd labeling; launching competitions to spur data set use; and revenue generation models for sustainability.


**five lessons**
1. motivations shape dataset
**Commercial** - creating new products for fundraising, dataset will give a moat, dataset will make a algorith more robust
**methodological** - benchmark for the field, data set we can figure out this method i'm curious about... 

**Applied** - how do i understand these data, how do i automate this annoying task 


2. transactional labels are always worse thank you think - 


3. find your place o the labeling system - anyone can label, experts only - messy middle - find your place on the lableing spectrum 

some strategies for the messy middle 
incentives, not just financial
new tools to make tasks easier 
chang the classifications 

4. don't ingnore shelf life - how long is your dataset good for? 
how long will this be a viable dataset? 

how stable are the biological processes 

5. think infrastructure not research 
ubiquitous, not bespoke
for a community, not a team 
a separate budget, not a budget line 
measure contributions - tracking usage, how much is data making impact 


e.g. imagenet - computer vision co.

---

4:30pm
**KEYNOTE**

Alix Dunn

Ethics and Consistency 
@alixtrot

data consistency - 

service optomiztion - benefits fo gorups of users 
redress - how redress is handled for what types of users and challenges 
data and interference 
monetization what is monetized when 


how values transfor decisions 

optomizing algorithm for a financial service - using values and parameters set by the organizations 
working through the process - would different taems make different decisions 

Consistency looks like: 
increaes alignment between values and actions 
guards against mistakes 
creates clarity for teams and users 
can be measure and improved. 

Types of mistakes:
errors fo ingnorance we don't know enough
errors of ineptitude proper use of what we know

components of consistency:
diverity
reflection
comparison
iteration 


thinking about consistenty:
having a real space for reflection 

comparison - making subjective decisions 
inter coder reliability - establishing ways to consistencly evaluate subjective situations


Iteration 
as you test your values - update your documentation, guidance, + values 

take learning process seriously - to improve over time 




# May 9 - Day 2

10:00am

**KEYNOTE**

**Teon L. Brooks**

Build, Empower, Grow

open source and data science work 

what does it mean to be human centered 
how dow we use data to empower, build and grow 


frition points in science in anlyses using tools 

The Negro motorist green-book - human data centered book - centered on the human experience 

example of how we build for users 

product discusssions 
Iodide + pyodide
Common voice 
CIEL and teh BrainWaves project 


MNE python - software for data analysis 
MEG+EEG Analysis and Visualization 


"your commits are a love letter from the past"

BIDS Brain imaging data structure 

OpenNeuro platform 

building team collaborations 



Iodide project 
narrative and code in a presentaable format 

take python stack and uses webassembly 
native compiled code on the web

Adam Rule 
Exploration and Explanation in computational Notebooks 

Pyodide

The first lanuage plugin for iodide 

upstream cpython 
numpy, pandas, matplotlib

webassembly 
fast way to run code on the web

related art
pypyjs
zero dependency python Google Native Client 
brython 

call for proposal for complier dev. 

Iodide project 
build tools to help you tell your story in a compelling adn interatve way 


alpha.iodide.io
github.com/iodide 


CommonVoice project mozilla 
community project 
related to free speech voice assistant projects in the US 

use of voice assistants 
 project deep speech - creating a voice reg. model , code in git repo 
 
 how to teach machines how people speak 
 
 CIEL cognitive innovation in education labs - new project 
 deliver high quality low cost hands on real research experience to underserved research communities 
 
 DIY Cog Sci 
 
github.com/teonbrooks

The brainwaves project 

 
 
 
 
 
 speech data, speech algorithims, compute 
 
 









11:00am

**Open Infrastructure for Open Science: How Binder Powers an Open Stack in the Cloud**
**Chris Holdgraf**

This talk will discuss the Binder Project in the context of open data and open science, two primary use-cases that have driven the project. It will cover the basics of the Binder Project, such as how to define a reproducible repository to share with others. It will then discuss one of Binder's core goals, which is to build on open standards to facilitate the use of *many* open languages, interfaces, etc. Finally I'll discuss how BinderHub, the technology behind a Binder deployment, is itself open source and deployable anywhere. I'll finish by describing a goal of distributed, federated BinderHubs that provide a network of reproducible data analytics environments.


public infrastructre

build open modular tools - public infrastructure 

jupyter levereages public infrastructure 
e.g. a jupyter workflow and standards 
package, notebook, protocols, kernels, reports 

scientific reproducibility and shareabliltiy 


Jupyter workflow
from you laptop to the cloud
some data sci should be taught to everyone  e.g. humanities and soc sci 
conceptual ideas around stats teaching 

how can we connect people with computation? 

Jupyter hub 

pre-config data sci environ. 

myhub.org


how can users package+share your work 

repotodocker.readthedocs.io 
create docker image package - to docker registry to share 


LIGO binder 

mybinder.org

pangeo - binderhub for earth
GeSIS


Jupyter-book 

publishable documents with pandoc 

Voila - quantstack  - dashboard for HTML 



Binder hub 

jupyterhub-team-compass.readthedocs












11:30am


Improving the Quality of Neuroimaging Scans


My presentation will be on how adjustments to the human connectome project (HCP) pipeline, with the use of the advanced normalization tools (ANTS), improved the data quality of neuroimaging scans provided by the Autism Brain Imaging Data Exchange (ABIDE). Autism spectrum disorder (ASD) is a neurodevelopmental disorder consisting of altered social and communication difficulties along with repetitive and restrictive behaviors. It is difficult to study a living brain safely which is why we use neuroimaging techniques such as MRI. Data quality can be affected by subjects moving in the scanner, or due to computing pipeline issues. Adjustments to the HCP pipeline lead to an increase in data quality, and a decrease in the amount of data lost. This will save researchers time, money, and data to study the neurophysiological aspects of ASD.

Autism SPectrum Disorder (ASD)

Data quality protocol 


neuro imaging is important to study the brain, 
ABIDE dataset is great, publically available for studying ASD

used for the efforts of properly studyhing ASD 




12:00 lunch 

----

12:30pm 
**Keynote**
Kristie Whitaker

The turing way sharing the responsiilty of reproducibility 


humans are the hardest part of reproducibility 
barrieris to reproducibility 

martin O'riely
make reproducible research too easy not to do 

Turing way online book 

practices at Turing should be...FAIR 
FAIR research data practices 

continuous integration 

continuous analysis 

CI makes you be explicit about what has changed 


Version control is a pre-req for almost everything! 


CI in ebook 

tools mentioned: 
repotodocker 
binderhub 

Turing binderhub 

CleverCSV package 

github.com.alan-turing-institute/CleverCSVDemo


A global collaboration 
m unsder
open leadership pronciples 

connect with the Carpentries 





1:30pm
Lightning Talks 


Stuart Giger bit.ly/ossdocs

FOSS free adn open source software

Vicky Steeves Gabriele Hayden librarians for reproducibility 
data management needed for reproducibility but doesn't guarantee it 

FLOSS reproducbility tools 

open knowledge maps





2:00pm 

**Data Science Training and Community Building through Hackweeks**
**Micaela Parker**

Informal training activities enable researchers at all levels to rapidly learn data science tools and best practices that fit their research questions and make significant advances in their work. In this talk, I will describe a highly successful informal training that has emerged in recent years called Hackweeks. These hackathon-style events place a strong focus on cultivating data science literacy, building a community of practice, and developing resources within an existing domain-specific community. By bringing together researchers from many different universities to address methods challenges within a research domain, Hackweeks take advantage of a shared language and shared scientific objectives. The Hackweek structure is designed to foster collaboration and learning among people from various stages of their career and technical abilities, and catalyze a community through a shared interest in solving computational challenges within a field (Huppenkothen et al, 2018). Hackweeks originally came out of the Astronomy community (Astro Hack Week, entering its 6th year in 2019) and the model has been successfully propagated to: neuroscience (Neurohackweek, now a 2-week NIH-funded program called Neurohackademy), geospatial sciences (Geohackweek), oceanography (Oceanhackweek), and more.


MSDSE 

Virtuous Cycle 

community learning within domains 

learning and pedogogy 
hackweeks shared language, shared scientific objectives 


goals of hackweeks 
foster data analysis literacy 
cultivate best proactices 
develop resources for an existing domain 

hackweeks format 
tutorials instrucdution, then project work 

participlant diversity 
Entrofy 

Participant selection 
based on user defined attributes 


wjp sussec go;k
hackweeks help resarcher, and enougarces them to work onpenly and towards reporductive results 






2:30pm


Beyond the WARC: Making Web Archives More Useful and User-friendly
Iiya Kreymer

Archives of the web contain not only web pages but any type of data. The only standard in web archiving is the ISO WARC file format, which specifies raw data captured from the web. However, the WARC files often lack any context or metadata about how this data was captured. The talk will briefly cover the basics of the WARC format, and also provide possible ideas for making web archiving data more user-friendly, present existing tools and suggest ideas for interoperable ways to describe collections and make sense of growing web archive data beyond the WARC format.


web archives can be small 

why web archive? 

the WARC file format 
WARC ISO standard 
limitations of WARC 
no index or records 
no defined data format 

accessing web archive 

fuzzy mathinvg rules 

---

3:30pm
**Version Controlled Stakeholder Reporting: Building an End-to-End Data Reporting Infrastructure**
**Jose M Hernandez**

King County, Washington is currently undergoing complex social and economic changes that have both positive and negative impacts on local residents. With rising rents displacing low-income households to outlying areas or into homelessness, there is a critical need to understand the prevalence and mechanisms of housing insecurity for government organizations tasked to address these issues. Currently, our team of Data and social scientists at the University of Washington, eScience Institute are collaborating with stakeholders across the King County Housing and Homelessness prevention agencies to derive meaningful insights from their data. While their aim is not to produce academic research, our findings may have significant and immediate impact for their organizational practices and the communities they are tasked to serve. In this context and where there is an iterative and constant feedback loop present, reproducibility of the results we present to them, from figures, tables, and even written language is critical. To ensure a successful collaboration, our team has built an end to end data reporting infrastructure to produce reports for our stakeholders that are reproducible and version controlled from raw data to final product. We employ some common open source tools to accomplish this, including R/Rstudio, Python, Rmarkdown, and git.



escience institute 
Carpentries 

project understanding housing instability and homelessness in King County 

exploring population that is homeless or at rist of being homeless and their interactions with human services provided thorugh serveral agencies 

data provided from 3 agencies 

s3buckets to store data in the cloud 



using data matching concepts to compare data 

software: 
python
Puget - hande PII cleaning , record linking , cluster improvements

https://github.com.uwescience/puget
built in python


Housing

https://github.com.PHSKC-APDE/Housing

King county Public health analyst did further further development to match it against public health data 

reporting in R 



aws_util
python

private repo
family of functions that processes the data from raw to linked longitudnal file 



analysis data output is CSV

using jupyter notebooks 
using rmarkdown for reporting - under version control to keep track 

all reports are private repos 

used carpentries lessons for training to move into more advanced training 


github.com/jmhernan


---

4:00pm

Spanking and Spreadsheets: Data-driven Sex Journalism
Jaquiline Nolis & Heather Nolis

When we saw that the Stranger, Seattle’s alternative newspaper, was running a survey on kinks and sexual preferences, we knew we had to get our hands on the data. We convinced the that using machine learning methods on the responses would be a good idea, and then we quickly set out to analyzing them. But we had never written an article for a newspaper before—nor had we worked with data even remotely as dirty. It turns out what makes for a good blog post or technical journal is very different than writing for print, especially for such a sensitive topic. In this talk we will cover how we made sense of the lewd data, the statistical methods we used (and failures we produced), as well as the final results that ended up in our feature article: “There Are Four Kinds of Sex Partners (which one are you).”


The Stranger Sex Survey responses used as survey 

data was on spss data

50qs 8000 responses 

5 things to decided analyze ideas 

training neural netwrok 

coming up with analysis topics - trying to find a data question

data apps and porn 
related kinks 
check out sexting
cross-tabs with funny questions

split th edata with k-means (kinks) 


data science and jounlanism 

http://bit.ly/sexdatascience







