[![Netlify Status](https://api.netlify.com/api/v1/badges/1862fcac-06ca-4df3-a311-0ead34a6bbb4/deploy-status)](https://app.netlify.com/sites/sustainable-building/deploys)
# Sustainable Building  Research Group Website using [Hugo](https://github.com/gohugoio/hugo)

The research group **Sustainable building** works with concepts, tools and strategies to 
enhance the sustainability performance of construction materials, building products, 
buildings as well as entire cities.  
The research is related to ecological and economic
life cycle assessment of construction materials, buildings and infrastructures, 
sustainability assessment tools for buildings, social-cultural and climate adapted 
design concepts as well as energy and material resource based building stock modeling 
and its visualization. 

[Live publication feed](https://swepub.kb.se/atom.jsp?q=(%27(WFRF:(N%C3%A4geli+Claudio+1987)%20OR%20WFRF:(Jimenez+Encarnacion+Divia+1989)%20OR%20WFRF:(Galimshina+Alina)%20OR%20WFRF:(Gonzalez+Caceres+Alex+Arnoldo+1982)%20OR%20WFRF:(Holger+Wallbaum+1967)%20OR%20WFRF:(Hollberg+Alexander+1985)%20OR%20WFRF:(Lanau+Maud+1989)%20OR%20WFRF:(Rosado+Leonardo+1975)%20OR%20WFRF:(Malakhatka+Elena)%20OR%20WFRF:(Melina+Forooraghi+1989)%20OR%20WFRF:(%C3%96sterbring+Magnus+1986)%20OR%20WFRF:(Quan+Jin+1983)%20OR%20WFRF:(Sanjay+Somanath+1994)%20OR%20WFRF:(Shea+Hagy+1982)%20OR%20WFRF:(Sjouke+Beemsterboer+1984)%20OR%20WFRF:(Toivo+S%C3%A4w%C3%A9n+1993)%20OR%20WFRF:(Xinyue+Wang+1995)%20OR%20WFRF:(Yutaka+Goto+1984))%27)%27&order_by=rank2&format=RIS)


Admin Guide for managing the site
=====================================================
Welcome to the administrative team of sb.chalmers!  

 This guide provides step-by-step instructions to set up your local environment for website management. Please follow these instructions carefully to ensure a smooth setup.

**Note**: If you find steps in this guide to be lacking, please update it to help future site admins navigate through using this project.  
**2021 - 2023**: [Sanjay Somanath](mailto:sanjay.somanath@chalmers.se)  
**2024 - 202X**: [Josie Harrison](mailto:josie@chalmers.se)  

Prerequisites
-------------

Before proceeding, ensure you have administrative access to the necessary GitHub repositories. Contact the current admin if you do not have permission.

Setting Up Your Local Environment
---------------------------------

1.  Clone the GitHub Repository

    -   To start, clone the GitHub repository to your local machine. This allows you to work directly with the website's code.

    
    ```bash
    git clone [https://github.com/SB-Chalmers/sustainable_building_website.git]
    ```

2.  Install Python 3.8

    -   Our website relies on Python 3.8 for various scripts and operations. Download and install it from the official [Python 3.8 release page](https://www.python.org/downloads/release/python-380/).
3.  Install Go 1.14.4

    -   Go is used for certain backend functionalities. Install Go version 1.14.4 from the official [Go downloads page](https://go.dev/dl/).
4.  Install Hugo 0.97.3 (Extended)

    -   Hugo is a critical component for running and building our website. Install Hugo 0.97.3 (Extended) from its [official release page on GitHub](https://github.com/gohugoio/hugo/releases/tag/v0.97.3).
5.  Update Your PATH Environment Variable

    -   After installing Python, Go, and Hugo, add their installation paths to your PATH environment variable. This step is crucial for using these tools from the command line.
6.  Verify Installations

    -   To confirm that everything is set up correctly, run the following commands in your terminal:
        -   For Python: `python --version` (should return Python 3.8.x)
        -   For Go: `go version` (should return go1.14.4)
        -   For Hugo: `hugo version` (should return v0.97.3/extended)

# Running Hugo

After successfully installing Hugo and setting up your local environment, follow these steps to run Hugo and start working on the website.

## Starting the Hugo Server

1\. **Navigate to the Project Directory**

   - Open a terminal (Command Prompt or PowerShell on Windows, Terminal on macOS and Linux).

   - Navigate to the root of the cloned GitHub repository using the `cd` command.
```bash
   cd path/to/your/repository
```

2\. **Run Hugo Server**

   - Execute the following command to start the Hugo server:

```bash
   hugo server
```

   - This command will start the Hugo server and make your site locally accessible. Hugo will provide a URL (typically `http://localhost:1313`) which you can open in a web browser to view your site.

3\. **Viewing Your Site**

   - Open your preferred web browser.

   - Enter the URL provided by Hugo (e.g., `http://localhost:1313`). You should see your website as it would appear online.

4\. **Live Reloading**

   - One of the advantages of using Hugo is live reloading. As you make changes to the website's content or design, Hugo automatically updates the view in the browser, allowing for real-time feedback.

## Making Changes

- When you edit files (like Markdown files for content, or HTML/CSS files for design), save them, and Hugo will immediately update the site in the browser.

- This is helpful for quickly seeing how changes will look on the live site.

## Building the Site for Deployment

- Once you are satisfied with your changes, you can build the static pages for deployment.

- Stop the server (if running) by pressing `Ctrl + C` in the terminal.

- Run the following command to build the static site:
```bash
  hugo
```

## Updating the site
Finally, make a commit with a helpful commit message and push to github.  
[Netlify](https://app.netlify.com/sites/sustainable-building/deploys) will then detect the changes and build a new version of the site and update it on the internet.

A good first change is to update the contact info on the website from the old admin to yours.

# Updating bibliography

The research group publications are managed through a combined .bib file (similar to one used in latex). There are many ways to get this but the one that we have been using is to leverage the swepub national database using a long and complicated atom rss request:

```
https://swepub.kb.se/atom.jsp
?q=(%27(
    WFRF:(N%C3%A4geli+Claudio+1987)%20OR%20
    WFRF:(Jimenez+Encarnacion+Divia+1989)%20OR%20
    WFRF:(Galimshina+Alina)%20OR%20
    WFRF:(Gonzalez+Caceres+Alex+Arnoldo+1982)%20OR%20
    WFRF:(Holger+Wallbaum+1967)%20OR%20
    WFRF:(Hollberg+Alexander+1985)%20OR%20
    WFRF:(Lanau+Maud+1989)%20OR%20
    WFRF:(Rosado+Leonardo+1975)%20OR%20
    WFRF:(Malakhatka+Elena)%20OR%20
    WFRF:(Melina+Forooraghi+1989)%20OR%20
    WFRF:(%C3%96sterbring+Magnus+1986)%20OR%20
    WFRF:(Quan+Jin+1983)%20OR%20
    WFRF:(Sanjay+Somanath+1994)%20OR%20
    WFRF:(Shea+Hagy+1982)%20OR%20
    WFRF:(Sjouke+Beemsterboer+1984)%20OR%20
    WFRF:(Toivo+S%C3%A4w%C3%A9n+1993)%20OR%20
    WFRF:(Xinyue+Wang+1995)%20OR%20
    WFRF:(Yutaka+Goto+1984)
    )%27)
    %27&order_by=rank2&format=RIS
```
This url need not be done manually, there is an excel file to do this (you will find the link to it in the notebook below)

There is a python notebook called `RG_Bibupdate.ipynb` in this repository that can help you update this bibliography. All you need to do is get the new bib and replace the existing bib file in this repo.

Then you need to run a hugo command to create a new page for each entry in the bib.
`academic import --bibtex library.bib`. These instructions are repeated in the notebook as well.

# WIP adding past masters thesis projects
There is a python notebook called `RG_MastersThesisUpdate.ipynb` in this repository that can help you scrape chalmers research and create new pages for the research group website


---

# Lycka till!

---