# Internal Linking Roadmap

**Goal:** Enhance SEO by adding 2-3 contextual internal links to each article within the "Internal Linking project" directory.

**Plan:**

1.  **Analyze Article Titles:**
    *   Objective: Get a high-level understanding of the topics covered in each article.
    *   Action: List all HTML files in the current directory and review their titles.

2.  **Create Tracking CSV:**
    *   Objective: Create a CSV file to track the internal linking progress.
    *   Action: Create a file named `internal_links.csv` with the following columns: `Article Title`, `Status`, `Link 1 Target`, `Link 1 Anchor Text`, `Link 2 Target`, `Link 2 Anchor Text`, `Link 3 Target`, `Link 3 Anchor Text`.

3.  **Read Article Content:**
    *   Objective: Understand the context of each article to identify relevant linking opportunities.
    *   Action: Read the content of each article to identify key topics, keywords, and concepts.

3.  **Identify Semantic Links:**
    *   Objective: Determine contextually relevant articles to link to from within each article.
    *   Action: For each article, identify 2-3 other articles that are semantically related and would provide valuable additional information for the reader. Consider the anchor text that would be most appropriate and contextual.

4.  **Implement Contextual Links:**
    *   Objective: Insert the identified internal links into each article using HTML `<a>` tags.
    *   Action: Use the `replace_in_file` tool to modify each HTML article.
        *   For each article, identify 2-3 suitable locations within the text to insert internal links.
        *   Create `<a>` tags with `href` attributes pointing to the target article's HTML file (e.g., `<a href="Target Article Title.html">Contextual Anchor Text</a>`).
        *   Ensure the anchor text is contextually relevant and naturally integrates into the surrounding sentence.

**Step-by-step Instructions:**

1.  **(Preparation)** Toggle to ACT MODE.
2.  **(List Files)** Use `list_files` tool to get a list of all HTML files in the current directory.
3.  **(Read Articles)** For each article:
    *   Use `read_file` tool to read the content of the HTML file.
    *   Analyze the content to understand the topic and identify linking opportunities.
4.  **(Identify Links)** For each article, determine 2-3 internal links to other relevant articles, considering contextual anchor text.
5.  **(Implement Links)** For each article:
    *   Use `replace_in_file` tool to insert the identified internal links with appropriate anchor text.
    *   Verify the links are correctly inserted and formatted in the HTML.
6.  **(Review)** After implementing links in all articles, manually review a few articles to ensure the links are contextual and working as expected.
7.  **(Completion)** Use `attempt_completion` tool to indicate the task is complete.
