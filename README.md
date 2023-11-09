# The Shawshank Redemption Film Website

This project is a website about the film "The Shawshank Redemption", selected from the IMDB 5000 Movie Dataset. The website is built with Bootstrap5 and consists of three pages: Movie Details (`index.html`), Actors (`actor.html`), and Director (`director.html`).

## Project Structure and Dependencies

My project strutures like this:

```
├── public
│ ├── imgs
│ └── videos
└── src
  └── styles
  ├── director.html
  ├── actor.html
├── index.html
```

- index.html: This is the deployment entry file.
- public: This folder is used to store static assets.
  - imgs: This subfolder within 'public' contains image resources.
  - videos: This subfolder within 'public' contains video resources.
- src: This folder contains the other HTML files and a 'styles' folder.
  - actor.html: An HTML file within 'src'.
  - director.html: Another HTML file within 'src'.
  - styles: This subfolder within 'src' is used to store Sass files and the CSS files.

There are three dependencies:

- Bootstrap 5
- Bootstrap Icons
- Google Fonts

To run the project, perform the following steps:

Local Setup:
(1) Open the "moviesJoy" folder using your preferred IDE.
(2) Run npm i to install the necessary dependencies.
(3) Install the Live Server extension and launch Live Server. Please note that opening index.html directly or not installing the dependencies may affect correct display.

Deployed Website:
The project is also available online at: https://student230011113-responsivefilm-codefreyy.vercel.app/

## Pages Summary

### Movie Details (`index.html`)

This page includes the movie name, release year, language, rating, duration, genre, director, actors, synopsis, poster, watch link, trailer, score, and popularity index.

### Actors (`actor.html`)

This page provides information about the actors, including their names, roles, biographies, photos, introduction videos, and lists of movies they've starred in.

### Director (`director.html`)

This page provides information about the director, including their name, role, biography, photo, introduction video, and a list of movies they've directed.

## Responsive Design

The project leverages Bootstrap's powerful responsive features. Mainly, the `img-fluid` class is used for responsive images, and the main body of the site is wrapped in a `container` element, which sets a max-width at each responsive breakpoint. This provides a consistent and adaptable layout across various screen sizes.

### Movie Details (`index.html`)

#### Navigation Bar

- For `lg` screens and above, all items are expanded, and the favicon is the full Netflix logo.
- For `md` screens, navigation items are hidden, replaced by a menu icon in the upper right corner. Clicking the menu icon reveals the menu items.
- For `sm` screens, the Netflix logo is replaced by a smaller 'N' icon.

#### Footer

- For `md` screens and above, the footer information is displayed in 4 columns, with the project and media icons (TikTok, Twitter, etc.) centered.
- For `md` screens and below, the footer information is displayed in 2 columns, aligned left.

#### Main Content

The main content layout varies depending on the screen size:

- `lg` screens and above: The content is divided into two rows. The first row has two columns: the first column has the movie title and movie information, and the second column has the movie score and popularity. The second row also has two columns: the first column contains the movie poster and other movie information, and the second column has the movie trailer.
- `md` screens: The first row's first column, containing the title and rating, is split into two rows. The second row's second column, containing the "trailer", is moved to the next row.
- `sm` screens and below: The second row's second column, containing the movie information, is moved to a new row below the poster.

### Actors and Director Pages (`actor.html` and `director.html`)

The top large image uses `img-fluid` for fluid responsiveness, and the content below is wrapped in a `container`. When the browser is reduced to `md` size, the character information and introduction video move from one row and two columns to two rows.

For `xxl` screens, the character's name appears in artistic font on the left side of the top image. When the screen is reduced to `xl` or smaller, this font disappears and reappears at the beginning of the next section.

## UX Design

The UI follows a clean, flat design with a dark/black theme complemented by a red accent color (#E83F3F) for a cool, cinematic feel. Various UX enhancements are also implemented, such as hover effects on links and cards, and a vertical scroll for long text sections.

## Accessibility

1. Aria-labels have been added where necessary, for example, on links and the navbar button toggler, to facilitate users with screen readers.
2. All images have `alt` text, videos have tracks, and form elements are associated with a `<label>` tag.
3. Clear link focus states are provided for screen readers.
4. Navigation across the page is fully supported with the `tab` and `shift + tab` keys.

A 'Back to Top' button has been added at the beginning of the footer. This allows screen reader users to navigate back to the top before reaching the less important links section at the bottom, in case they want to start browsing from the top again.

## Validation

The website's HTML and CSS have been validated using the [W3C validation service](https://validator.w3.org/#validate_by_input) with no warnings or errors.The website's HTML and CSS have been validated using the [W3C validation service](https://validator.w3.org/#validate_by_input) with no warnings or errors.
