# Instructions for New Developer on Internal Linking Project

This document outlines the steps taken so far in the internal linking project, and provides instructions for continuing the work.

## Project Goal

The goal of this project is to enhance the SEO of a collection of blog articles by adding 2-3 contextual internal links to each article.

## Current Progress

1.  **Project Setup:**
    *   The project repository has been initialized and the initial content has been pushed to GitHub: [https://github.com/seoninja13/internal-linking-proj.git](https://github.com/seoninja13/internal-linking-proj.git)
2.  **Roadmap Creation:**
    *   A `roadmap.md` file has been created to outline the plan and step-by-step instructions for the internal linking process.
3.  **Tracking CSV:**
    *   An `internal_links.csv` file has been created to track the progress of the internal linking process. This file contains the following columns:
        *   `Article Title`: The title of the HTML file.
        *   `Status`: The current status of the internal linking for the article (e.g., "Not Started", "In Progress", "Completed").
        *   `Link 1 Target`: The filename of the first article being linked to.
        *   `Link 1 Anchor Text`: The anchor text used for the first internal link.
        *   `Link 2 Target`: The filename of the second article being linked to.
        *   `Link 2 Anchor Text`: The anchor text used for the second internal link.
        *   `Link 3 Target`: The filename of the third article being linked to.
        *   `Link 3 Anchor Text`: The anchor text used for the third internal link.
    *   The `internal_links.csv` file has been populated with the list of HTML files in the project, with their status set to "Not Started".
    *   Internal linking has been added to "Automate Your Kitchen A Guide to Automated Appliances.html", linking to "Design the Perfect Culinary Prep Station for Your Home Kitchen.html" with the anchor text "robotic cooking devices".

## Next Steps

1.  **Select an Article:** Choose an HTML file from the `internal_links.csv` file that has a status of "Not Started".
2.  **Read Article Content:** Use the `read_file` tool to read the content of the HTML file.
3.  **Identify Semantic Links:** Analyze the content to identify 2-3 internal links to other relevant articles, considering contextual anchor text.
4.  **Implement Contextual Links:**
    *   Use the `replace_in_file` tool to insert the identified internal links with appropriate anchor text.
        *   For each article, identify 2-3 suitable locations within the text to insert internal links.
        *   Create `<a>` tags with `href` attributes pointing to the target article's HTML file (e.g., `<a href="Target Article Title.html">Contextual Anchor Text</a>`).
        *   Ensure the anchor text is contextually relevant and naturally integrates into the surrounding sentence. You may need to rewrite the sentence slightly to make the link fit naturally.
    *   Update the `internal_links.csv` file with the target articles and anchor text used for each link, and change the status to "In Progress".
5.  **(Repeat)** Repeat steps 1-4 for each article in the `internal_links.csv` file.
6.  **(Review)** After implementing links in all articles, manually review a few articles to ensure the links are contextual and working as expected.
7.  **(Completion)** Use `attempt_completion` tool to indicate the task is complete.
