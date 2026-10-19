# Multi-page Website Deployment

A simple, responsive multi-page website built using **HTML5** and
**CSS3**. The project includes Home, About, Services, and Contact pages,
with shared navigation and responsive styling.

## Project Objective

To create a multi-page website using HTML and CSS, manage the source
code with Git and GitHub, and deploy the static website using Amazon S3.

## Features

-   Four linked pages: Home, About, Services, and Contact
-   Shared navigation menu
-   Responsive layout for desktop and mobile screens
-   Services displayed using CSS Grid
-   Consistent styling with a shared CSS file
-   Contact form design (front-end only)

## Technologies Used

-   HTML5
-   CSS3
-   Git
-   GitHub
-   Amazon S3 Static Website Hosting

## Project Structure

``` text
multi-page-website/
├── index.html
├── about.html
├── services.html
├── contact.html
├── style.css
└── README.md
```

## Run the Website Locally

1.  Download or clone this repository.
2.  Open the project folder in Visual Studio Code.
3.  Open `index.html` in a browser, or use the Live Server extension in
    VS Code.
4.  Use the navigation menu to visit the other pages.

## Deploy on Amazon S3

1.  Sign in to the [AWS Management
    Console](https://console.aws.amazon.com/).
2.  Open Amazon S3 and create a uniquely named bucket.
3.  Upload `index.html`, `about.html`, `services.html`, `contact.html`,
    and `style.css`.
4.  In the bucket's **Properties**, enable **Static website hosting**
    and set `index.html` as the index document.
5.  Configure access carefully. If using a public S3 website endpoint,
    allow only the public read access required for the website files.
    Alternatively, use Amazon CloudFront with a private S3 bucket.
6.  Open the website endpoint shown in the Static website hosting
    settings and test every navigation link.

**Note:** An S3 static website endpoint uses HTTP. For HTTPS, consider
Amazon CloudFront. AWS usage may incur charges, so review pricing and
remove resources you no longer need.

## Git Commands

To upload future changes to GitHub:

``` bash
git add .
git commit -m "Update website"
git push
```

## Testing Checklist

-   [ ] All four HTML pages open correctly.
-   [ ] Navigation links work on every page.
-   [ ] CSS styling loads on every page.
-   [ ] Layout works on desktop and mobile screens.
-   [ ] Website works from the deployed endpoint.

## Limitations

The Contact form is currently a front-end design only. It does not send
or store messages because no backend or form-handling service is
connected.

## Conclusion

This project demonstrates how to build a basic responsive website with
multiple HTML pages, style it with CSS, track changes with Git/GitHub,
and deploy static files on Amazon S3.

------------------------------------------------------------------------

**Project:** Project Statement 18 --- Multi-page Website Deployment
