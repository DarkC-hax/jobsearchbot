# Job Search Bot

The goal of this software is to semi-automatically help me apply to cybersecurity jobs. The use-case for this software is I will run it every Monday, Wednesday, and Friday and apply for new jobs.

- Have a pre-set list of job board queries for linkedin, glassdoor, google jobs board, and a few more. 
- The software uses a web scraper to get job listing data from the google jobs board and all these other queries
- The software should automatically reject jobs 4 or more days old, and (saving rejected jobs) jobs that have been rejected before, as well as jobs that match some other requirements like age etc. 
- The software, when it comes upon a viable job candidate, will present it to me for manual review. 
- In this case, the software should also do some OSINT research on the company itself and come up with a few base metrics (employee count, what the company does, where are offices close to me, who are relevant employees and how can I contact them, etc.), as well as opening the job application link in my browser for manual review, at which point it asks me to proceed once more
- If I proceed with the job, the software should dynamically edit my LaTeX resume and generate a cover letter and an email to recruiting from a template, both using the OpenAI ChatGPT API. 
- It will then ask me to review and suggest changes manually to the resume, which will loop back into OpenAI's ChatGPT API once more until I am satisfied.
- When I'm satisfied, it dumps the relevant files into a folder and opens the job application link for me.
