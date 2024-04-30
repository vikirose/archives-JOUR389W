# llm-archives

### Instructions

Click the "Use this template" button for this repository and choose "Create a new repository". You can give it the same name (llm-archives).

Once it's ready, go to [Groq](https://console.groq.com/keys) and follow the directions to get an API key. You'll need to login (or create an account if you don't have one).

Copy the API key value and then click on the Settings of your GitHub repository and click on "Secrets and variables" on the left side, then choose "Codespaces"

Click the green "New Repository Secret" button and paste your API Key into the "Secret" box, then put GROQ_API_KEY in the Name box above it. Click "Add Secret" and click on the name of the repository to return to the main page.

From there, click the green "Code" button and create a new Codespace in the Codespaces tab.

In the Terminal type the following: pip install requests groq and hit enter.

Then type: python get_stories.py

You should see a file called cns_maryland_posts.json appear. Let's look at it. It contains some details of the past 10 CNS stories.

Back in the Terminal, type: python entity_extraction.py and watch the output.

### Evaluation for JOUR389W

PUT YOUR EVALUATION HERE
I used this Baltimore Banner article https://www.thebaltimorebanner.com/economy/science-medicine/us-malaria-research-mosquitoes-C5HEXKNL4NBOJFGVKRZG2BHPA4/ I bumped the output against the article and it seems to have grabbed the few items requested sucessfully. For this article in particular it gave only a few people but many locations and organizations. Some of the organizations I might have put as locations such as the Malaria Research Institute. For the use of the organization, a line of what tags to extract would have to be defined up front. For most news orgs any holidays, titles, topic, maybe reoccouring words in a article might be helpful. For this article things I would request to ID animals, plants, insects, medical diagnosis, habitats, climates, symptoms, contacts, statistics, and numbers. Some or most of these tags would not apply to all articles, but may be a useful subset so picking and choosing what info is extracted could be crucial in archiving. 