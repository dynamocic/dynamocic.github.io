# Dynamo website 

## Where to find text for different webpages

- `index.markdown` defines the layout of the main landing page. This includes inserting information from other files into the rendered webpage. So the header image comes from `media/tube.jpg` and the opening hours come from `_includes/hours.md` for example. 

- `_data/header_navigation.yml` defines which pages can be accessed in the header menu. In this file, the title (e.g. Events) is the name that you click on the website. The url is the url extension from the website corresponding to the page. For `events.md` the resulting url extension is `events.html` for example.

There are currently four main pages:
- `events.md` for events
- `survey.md` for the lending library survey
- `nuts.md` for the nut allergy alert 
- `lendinglibrary.md` for information about the lending library

## Some basics

Files with a `.md` extension are markdown files. Markdown is a language that allows you to write plain text and use specific (combinations of) characters to format the text. This is then compiled to html when it becomes the website version. Here are some basics if needed: [https://www.markdownguide.org/basic-syntax/](https://www.markdownguide.org/basic-syntax/).

Within the `.md` files, the top specifies a title - for example `lendinglibrary.md` has the title Lending Library. This is the title of the page which you will see when you hover over the website tab in your browser. It is **not** the title of the page which appears in the header menu.

Titles for the header menu are specified in `_data/header_navigation.yml` instead. 

## How to update text on a webpage

1. **Find the file** that corresponds to the page and open it by clicking on it. This opens the plain html preview of the code.
2. **Edit the file.** There should be a little pen icon somewhere in the top right. This opens the Edit window with the code. You can also switch to the Preview tab so you can check if the formatting is working as expected.
3. **Optional: edit additional files.** If there are multiple 
4. **Commit changes.** Once you're happy with your changes, you should commit the change. By default, the commit message will describe which file you updated and it commits to the `main` branch. You can change the commit message and/or add an extended description to describe which changes you made. This is helpful in future when you want to understand changes you made previously.
5. **Check website deployment**. After you've committed the changes, the website should be rebuilt automatically. At the top of the GitHub repository, go to Actions. You should see a process called *pages build and deployment* with a timestamp that corresponds to your commit. If you go to Actions immediately after committing your changes, you may see that the process is still running. If it's (been) successful, you'll see a green tick mark next to the process. This means the website should be up and running correctly, with your changes applied to them.
6. **Check website**. Go to the webpage and make sure that everything has been changed as expected. Repeat the process if necessary.
