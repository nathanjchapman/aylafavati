# README

## Site Structure

In the top folder (`aylafavati/`) you will see the following items:

- `images/`
- `music/`
    - `index.html` (your music home page)
- `pdfs/`
    - `CognitiveDissonanceDocument.pdf` (this is referenced in `research/cognitive-dissonance.html` on line `76`)
    - `Resume.pdf` (this is referenced in every page in the `<footer>`)
    - `ThesisDraft.pdf` (this is referenced in `research/loudness-metering.html` on line `61`)
- `research/` (put your case studies here)
    - `cognitive-dissonance.html`
    - `feedback-loop.html`
    - `loudness-metering.html`
    - `template.html` (template case study with different blocks of content)
- `scripts/`
    - `index.js` (contains the code for the `to-top-button`)
- `styles/`
    - `normalize.css` (a library that fixes some funky  CSS defaults)
    - `main.css` (All of the styles for the site)
- `about.html`
- `index.html` ← this is the **home** page!
- `README.md` (your reading this right now)


## Adding a New Case Study

1. Duplicate `/research/template.html` in the research folder.
2. Rename it to your case study title.
    - Use lowercase words seperated by dashes. You can use: https://slugify.online/ to past any title and it will format it for you!
3. Populate the file with your content! (Use the other case studies as reference for how to format and include different items.)
4. Create the card in the home page (`index.html`)
    - copy the following:
    ```html
    <article class="case-study-list-item">
        <img class="case-study-image" src="/images/THUMBNAIL.png">
        <div>
            <h2>TITLE</h2>
            <p>DESCRIPTION</p>
            <a href="/research/TITLE-SLUG.html">read more →</a>
        </div>
    </article>
    ```
    - paste above or below one of the article elements in `index.html` (home page)


## Publishing Changes

- Open the Terminal app and navigate to the project on your computer using (example: `cd /Documents/Development/aylafavati`)
    - If you have the folder already open in finder, in Terminal you can type `cd ` (add a space), the drag and drop the folder from Finder into the Terminal and it will paste the directory path and you can press `enter` to navigate there.
- Open the Folder in Sublime Text
- Make your changes, save the files.
- Now back in your terminal you can type `git status` to see the files that were edited.
- Type `git diff` to see the changes made.
- To save your changes:
    - `git add .` press `enter`
    - `git commit -m "Brief, one line description of your changes"` press `enter`


## Image Sizes

- Whenever you are going to add any images (primarily thumbnails and figures for case studies)
- Make thumbnails 700x700 pixels
- Make figures no less than 1200px wide (the height can vary).
    - If you want three small images side by side: combine them into one larger image (see: `images/PrototypeIterations.png`.
