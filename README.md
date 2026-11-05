# My Portfolio

A personal portfolio website showcasing software-development coursework and GitHub projects.

## Languages and libraries

- **HTML5** for page structure, navigation, project sections, and the contact form.
- **CSS3** for styling, responsive images, the welcome modal, tooltip, and dark mode.
- **Vanilla JavaScript** for DOM manipulation, form feedback, project objects, and browser storage.
- **Libraries/frameworks:** None. The site uses browser-native features only.

## Features

- A welcome modal with a Close button.
- A hover/focus tooltip on the Contact form's Submit button.
- A Dark Mode toggle saved using `localStorage` across page loads.
- Three JavaScript project objects, each containing a title, short summary, image path, and GitHub repository URL.
- Project data saved with `JSON.stringify()` to `sessionStorage` and restored with `JSON.parse()` on later loads within the same tab session.
- Project cards created dynamically with DOM methods such as `createElement()` and `appendChild()`.
- A contact form that shows a simulated confirmation after two seconds. **It does not send an email or save submitted messages to a server.**

## Requirements and setup

- A modern browser with JavaScript, `localStorage`, and `sessionStorage` enabled.
- No package manager, build step, external JavaScript library, database, or API key is required.
- Keep `index.html`, `project.css`, and the `images` directory together.
- The image files expected in `images/` are:
  - `ProjectGithubSSS.png`
  - `ProjectGithubPython.png`
  - `ProjectGithubShenron.png`

## Run the site

Open `index.html` in a browser. For more reliable browser-storage behavior, use a local development server (such as VS Code Live Server) instead of opening the file using `file://`.

## Test session storage

1. Open the site and close the welcome modal.
2. Open browser Developer Tools → Application → Session Storage (or type `sessionStorage.getItem("portfolioProjects")` in the console).
3. Confirm the `portfolioProjects` key contains a JSON array of three projects.
4. Refresh the page and verify the three project cards still appear.
5. Toggle Dark Mode and refresh to verify the saved preference persists.

`sessionStorage` is generally scoped to the current browser tab and origin and is cleared when that tab's session ends. `localStorage` generally persists across browser restarts unless cleared.

## Project repositories

- [Sara's Shirt Shop](https://github.com/sarfie5786/Storefront-website)
- [Python for Data Analytics](https://github.com/sarfie5786/Python)
- [Shenron](https://github.com/sarfie5786/DBZ)
