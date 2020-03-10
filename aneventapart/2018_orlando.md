# An Event Apart

## Beyond Engagement

- always have the clients intentions in mind when creating a product or feature
- how quicky can you solve the customers problem
- Design CPQ (Content Performance Quotient)
  - purpose driven design and content
  - time it takes the client to get the info it came for
- every site should immediately convey to the client what the site or businesses main function or intent intentions
- Pretty garbage
  - garbage in a delightfully responsive grid is still garbage
- slash your architecture, shrink your content
- ask why do we need this and compare your goals
  - does your product have clearly defined goals?
- every design is intentional
- if your deisgn isnt going somewhere its going nowhere
- real estate metaphor
  - large house, tokyo apartment what is most important to client
  - think of necessities
  - small screen is a metaphor for the customers attention
- put content where your customers will see it
  - video? youtube
- give the person what they absolutely need and build upon that
- just in time information is better then bombarding clients with information
- atomic design
  - focus relentlessly on the individual interaction
- waterfall method
  - go thru all content on site create cards of content
  - massive content inventory
- agile/scrum
  - constantly iterate on content
  - best bet: inhouse team
- redesign
  - opportunity to start fresh
  - best bet: outside team
- which sites should be fast? slow?

## Digital Marketing Strategies for the Busy Web Master

- 10,000 days of the Web
- social media is only 3,000 days old
- average time spent on social media 1hr 45min, website we work on 15 seconds
- vanity metrics
  - throwback to hit counters
  - likes
- think about your audience and see if your post schedule makes sense for your industry
- check your personal bias
- there is a practicioneership to social media
- look through app store and review top social media apps
- 85% of snapchat 158 million daily active users are 15-34
- by 2019 video will account for 80% of all consumer internet traffic
- for eccomerce site add page for discounts for clinet doesnt have to go to web to find
- convert clients early in buying cycle
- long tail conversion
- facebook pixel make sure to add to site
- marketers who use video convert 49% more
- 50% of Faceboook video content is viewed on mobile
- 85% videos are viewed without sound
- SRT Edit Pro - subtitles for video
- it all comes down to the creative for social engagements
- google ad words
  - must turn on conversion metrics
- review trends.google.com
- google my businesses
- instagram
  - 800 million monthly users
- social networks change their algorithms to deal with the "problems of success"
- hashtagify for relevant hash tags
- hash tags should be seperated from original post
  - style is seperate from markup
- archive can be used to remove unrelevant posts
- planoly instagram visial management platform
- influencer marketing
  - 33% trust ads, 85% trust peers
- lefty.io to find influencer
- 25k followers average sponsored post rate $180, 5.30% average engagement rate
- design once use everywhere
- spyfu to check out competitor keywords

## Scenario Driven Design Systems

- design doesnt scale
  - Stanely Wood
- u.s. web design standards
  - playbook.cio.gov/designstandards
- design system
  - collection of resusable components
  - a system is an interconnected set of elements cohnrently organized in a way that achieves something
  - feels cohesive, unified, connected
- start your design system with user-scenarios
- in order to create a flexible system you must be specific
- successful design patterns dont exist in a vacuum
- successful design systems start with content and people
- scenarios, not layout, should drive variation
- no hypothetical systems
  - dont try to anticipate what the user might do
  - focus on current behavior and what they need to accomplish
- UI inventory
  - Brad Frost
- Purpose-Directed inventory
  - Alla Khlomatova
  - smashingmagazine.com/design-system-book
- presentational differences vs semantic differences
- identify core workflows and the patterns that need to support these workflows
- know your use case
- shopify polaris design system
- lede image?
- components can have multiple variations based on consumer
  - venue card
  - game card
  - product card
- name components collaboratively
- establish shared common language
- foundational elements + room for customization
- good vs bad variation
  - good
    - specific need
  - bad
    - visual variation

## CSS Grid

- main concpets to understand
  - Cascade, Inheritance, Specificity
- block and inlince axis
  - block horizontal
  - inline left and right and vice verse
- browser knows max and min content size
  - width: max-content; or width: min-content;
- flexbox is staring from max-contnet ank taking space away
- grid starting at min-content and adding space
- max-content will lead to overflow of content
- fit-content can be passed a size (15ch) 15 characters
- 12 and 16 column grids are fairly standard
- 63% of survey respondents support IE10+
- for desktop browsers supporting the last 2 versions of browsers is common
- new grid 2.0 will have the use of subgrids
- many of the browsers without support are most popular with areas where data is expensive and devices are less capable
- feature queries in CSS
  - test for support of different browsers (flexbox, grid, etc)
- statcounter.com?
- the new css layout by rachel andrew

## Making Sense of New CSS

- feature queries need a property and value?
  
``` css
@supports (--css: variables) {
        stuff goes here
    }

```

- @supports (display: grid) {
    ...
     @supports (writing-mode: sideways-lr) {
         ...
     }
}
- @supports (display: grid) {
    ...
}
@supports (display: grid) and
(writing-mode: sideways-lr) {
    ...
}
- a couple options for media querioes
- MOSS (Media Outside Supports Statements)
  - When there are more media swithces than support blocks
  - When @upports are used for a few cutting edge features
- MISS (Media Inside Supports Statements)
  - when there are more support blokcs than media switches
- flexbox has wider browser support than rounded corners (border-radius) around 98%
- flexbox is dependant on writing direction
  - flex-start will render either left to right, right to left, etc based on country writing direction

## Variable Fonts

- form and shape of typoography shapes how we emotinally connect with it
- styleguides.io
- shopify Polaris system
- 99% invisible podcast
- design systems need to be flexible and not so ridigd that it cant accomomdate different sizes
- introduced two years ago
- a single font file that acts as many
- type can be changed using css
  - x and y variables are exposed to me manipulated by css
- chrome is only browser that is not supporting but there are a couple work aroujnds
- as a font developer you can specify default settings and max weights for the font face
- Jason Pamental wrote the variable fonts guide on MDN
  - nightly.mozilla.org
- Tim Brown
  - css locks
  - typekit designer
- play.typedetails.com
- Mark Simonson
  - Proxima Nova typeface
- research monotype? type company?
- check Jason's github and codepen for examples
- <https://www.axis-praxis.org/>
- <https://wakamaifondue.com/>
- <https://developer.mozilla.org/en-US/docs/Tools/Page_Inspector/How_to/Edit_fonts>

## Name That Script

- consider the impact of third party scripts, designing and delivering a great expereince isnt enough
- categories of third parties
  - advertising, ab testing, analytics, social media, cdn, custoer info, comments, essential (jquery. chart.js, etc)
- ghostery.com
- itemizing scripts or ategorizing, use a htttp archive format website.har(json)
- network request panel, save all as HAR
- har.tech
- charlesproxy.com
- requestmap.webperf.tools.com or requestmap.webperf.tools
  - request visual anylizer
- request map can also export csv
- builtwith.com
- know industry standards
  - alexa top u.s. sites 50 (46 with work firendly site)
  - 213 thord part domain urls
  - 22 average per site
  - ad services were the top, demdex.net?
  - nytimes 64
  - washingtonpost 63
  - chase 12
  - news and shoppnig had the most
- better.fyi/trackers
- trentwalton.com
- does your site depend on third party functionality
- 25-40% U.S. Internet users block ads
- research GDPR(General Date Protection Regulation)...linked to cookies and cookie notifications on sites
- remarketing
- smashingmagazine.com for gdpr resources
  - privacy by design (smashingmagazine)
  - privacy impact assessment (gsa.gov)
- tag managers will allow access to add additional scripts to site
- account for third party scripts during prototyping
- audit third parties
- monitor performance
- competitive analysis
- gather compelling results
- wpostats.com
- comparative data
  - webpagetests.com
  - can be used to compare loading of certain scripts
- use real user monitoring tools

## Inclusive UX

- doing this in pencil allow us to quickly prototpe and throroughly document any iteraction that the intented feature might needed
- creating the high fidelity preview is akin to creating a mockup and basing user interaction based on that
- we review wireframes for thier predictive and preventative value
- storyboards help surface disagreement earlier in the process
- assebility is an outcome, inclusive design is a process
- intentional facilitation and crafting of interactions withing an ecpsystem that incprporates inclusion as a core value
  - inclusion must be a core value
- techniques for teams
  - 1.better communication
  - layer of annotations on top of wireframe
    - have a specific focus order
  - the core value of a wireframe is in the conversation, not in the boxes
  - 2.reverse engineering
  - helps you see opportunites for better discussion
  - 3.interaction tables
  - there is value in the reference and value in creating it together
  - 4.practice inclusive design
  - include people with disabilites in the process
  - usability studies have helped us learn
    - WCAG2.1 non-text contrast
  - WCAG2.1 is the accessibility standard
  - luild cta into links
  - visibile label of something on the screen should be in the link
  - design with people with disabilites, not for people with disabilities
  - dont stop with just colors for color pallettes, add documentation for good combinations, large font, and possible things to avoid
  - add contrast ratio
  - anything liess than 3:1 we should avoid
  - color palletets should include both good and bad combinations
  - slide to confirm is pretty cool, very intentional action
  - add another gesture that will relfect the intent for the design
  - a carousel vs a list or grid
  - 5.css class name review
  - use aria class names to signifiy intent of the interface
  - review in high contrast - chevron down
  - transparent borders on pop outs
  - look for things that are meaningful in the design
  - consider complementary things to use iwth gestures
  - accessibility is an outcome, incluse design is a process
  - embrace the process

## Leveling Up Your Design Communication @aaron

- as languages intesifies
- language shapes the work, the culture, and partnerships
- design is a team sport
- building soft skills is key
- language and communicaiton is huge in our careers
- language or terms to add to lexicon
  - visibility
- communication flows best whrn the work is visible  
- design that's not visible can't be valued
- "make space" book on amazon
- design reviews: formal assement of work
- design reviews are the heart of any design team
- invite the right people, not just designers
- review influential people to design reviews so work always remain visible
- limit attendees to 5-6 people to be productive
- design reviews need a facilitator to help guide the process
- google ventures process
  - set the stage (email)
  - review business goals (the why, this is why it helps the biz)
  - review the customer/client goals
  - review constraints
  - review schedules
  - set expectations on fidelity
  - direct the feedback
    - make sure to frame quesitons that you need answered up front
  - feedback
  - be specific
  - tie everything to goals
  - affirm whats working
  - problems first, then solutions
  - suggestions, not mandates
- cadence: rhythmic flow
- creating aculture of feedback
- apple design review cadence
  - kind of like saturday night live
  - monday staff meeting - define the work
  - tuesday team reivews of rough drafts
  - wednesday: work day
  - thursday: team revies refined work
  - friday: pencils down, executive review
- do we do design sprints?
- polish: improve. refine, or add the finishinng touches to
- retrospectives: looking back on or dealing with past events or siutations
- learn from every succes and failure
- how matt spiel from lyft runs retros
  - survey before the meeting
  - rate team and individual performance
  - start, stop, keep
- the infrastructure
- agile islands 1:11 (one designer with 11 engineers)
- paired design: a set of two things used together or regarded as a unit. two people related in someway or considered together
- diogenes brito slack designer
- design operations: a piece of organized and concerted activity involving a number of people, especially members of a design team
- designops handbook at designbetter.co
- safe harbor: protected from or not exposed to danger or risk; not liely to be harmed or lost
- the organization
- translation: a written or spoken rendering of the meaing of a word, speech, book, or other text into another language
  - tie things back to what is relevant to your audience
- speak to business goals not design goals
- design debt slows time to market
- ux crashes reduces retention
- how should we be measuring a design teams success
  - heart framework
  - happiness, engagement, adoption, retention, task success
- co-creation: the action or porcess of bringing something into existence together
- design-centricity develops by inviting participation into design
- jake knap? design sprints book
- enterprise design sprints (DesignBetter.Co)
- internal workshops
- workshops are good for getting peoples buy-in
- create a shared language and process
- language thrives when its supported by a process
- build partnerships more effectively

## The New Design Material @bigmediumjosh

- how do we use technology in a way that adds meaining
- how do we think of machine learning as a design material
- five categories that machine learning can ad value
- recommendations
  - slack finds people based on interests
  - predictive typing
  - google form classifications based on questions text
- classification
  - washington post bots writing basic articles
  - system they use is called heliograf
  - mural (post it note example)
- clustering: organize and group thinfs (people, concepts)
  - identify incisible patterns
- generation
- <https://airbnb.design/sketching-interfaces/>
- what tools and techniques do we use
- match a human need to a machine skill
- google cloud model ml
- microsoft custom vison
- review public api's in link
- lobe app (lobe.ai)
- topbots.com/ ai community website
- what is its grain?
- the machines are weird so diesgn for failure and uncertainty
- our job is to set expectations and
- B.A.S.A.A.P (be as smart as a puppy)
- narrow domains
  - what can the machines focus on
  - narrow problems dont have to be small problems
- signal your intention, reveal your action
- the machines reinforce normal, what is normal is garbage
- weapons of math destruction (book)
- kranzburgs first law
- the more we talk to robots the more talk like robots
- mindfultechnology.com, juvetagenda.org, bigmedium.com
