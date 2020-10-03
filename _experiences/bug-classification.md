---
title: Automated Assignment of Bug Reports using Natural Langauge Processing 
image:
  path: /assets/images/softmax.jpg
  thumbnail: /assets/images/softmax.jpg
---
As a Product Management Intern at Pegasystems, a fellow intern and I built an [NLP-based classification system](https://github.com/kenneym/bug_classification_research) to read bug reports sent to Pegasystems and automatically assign those bugs to be resolved by the relevant engineering teams. The model reads in said reports in email (HTML) format, processes them and analyzes them, and attempts to identify specifically which engineering team would be best suited to solve the bug at hand. 

In order to accomplish this task, our model must identify words and phrases within the email that can help identify where exactly the customer's problem may be originating with respect to Pegasystems' technology stack. If a bug report contained a significant number of terms related to cloud technology, for example, our classifier may classify that bug as being best addressed by the cloud engineering team at Pegasystems. Likewise, if a bug report contained references to UI elements ('button', 'sidebar', etc.), our classifier may determine that the bug is best addressed by the UI engineering team at Pega. To accomplish this task, a deep learning model was constructed to assign any given bug report to 1 of 47 different engineering teams.

Prior to the creation of this machine learning model, Pegasystems employees relied on manually assigning bug reports to the relevant engineering teams so that bugs could be investigated and resolved. This machine learning model will help to free up human work-hours for other tasks at Pegasystems, to prevent the accumulation of unresolved bugs (by assigning bugs immediately after they are recieved), and to address potential issues in Pega's technology stack more quickly and effectively. It comes with an estimated cost savings to the company of 1MM+ per year, by recoving many man hours that were formerly spent on bug classificaiton.

After building this product, I was given the opportunity to lead a team of 7 engineers to deploy this model to production. After working with this team for a month and a half, the model was successfully deployed and remains in use at Pegaystems today. Click the Github icon to see a preliminary version of the model which has been open sourced &rarr; {% include icon-github.html username='kenneym/bug_classification_research' label=' '%}
