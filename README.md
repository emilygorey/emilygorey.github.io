# Emily's Personal Website

Developed and documented by [ng-david](https://github.com/ng-david)

## Updating Website Colors

1. Open `/_sass/_variables.scss`

2. Edit the hex color values for `$brand-color` and `$brand-color-dark`

## Updating Home Image

1. Put your new image in the folder `/img/`

2. Open `/css/main.scss` and find the line `article.home {`

3. Between the curly braces ({}) that follow, there should be a line that says `background-image: url('/img/<arbitrary_image_name>.jpg');`

4. Replace the `<arbitrary_image_name>.jpg` with the name of your new image.

## Updating About

1. Edit the text in the file `/about.html`

## Updating Resume

1. Upload your resume with **public** access on Google Drive

2. Follow this tutorial to get the <iframe> embed code from Google Drive: [link](http://www.alicekeeler.com/2016/06/05/google-drive-embed-pdf/)

3. Update the <iframe> tag in `/resume.html` with your newly generated one

## Update Portfolio

TODO: make portfolio have a separate image folder

## Writing a New Blog Post

1. Create a new file in the directory `/blog/_posts/<FILENAME>`. The new file must be named in this standard format: `2016-07-26-name-of-your-post.md`

3. Copy paste the template file's contents (`/blog/_posts/blog/_posts/TEMPLATE.md`) into your new blog post file.

4. Replace the contents with your new post's contents.

5. Congratulations, you've made a new post!

DAVID TODO: Make better instructions for this...

## Update Contact Email

1. Open `/contact.html`

2. Find the line that says `<form class="contact-form" method="POST" action="http://formspree.io/<arbitrary_email@gmail.com>"`

3. Replace `<arbitrary_email@gmail.com>` with your new email

4. Try sending a test message to yourself

## For Local Development Purposes:

1. Run `$ bundle exec jekyll serve` to serve the website locally at port `4000`

2. Open browser at `localhost:4000` and begin developing!
