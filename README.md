# Emily's Personal Website

Created by [ng-david](https://github.com/ng-david)

---

### Updating Website Title and Description

1. Open `/_config.yml`

2. Change text next to `title:` and/or `description:`

---

### Updating Website Colors

1. Open `/_sass/_variables.scss`

2. Edit the hex color values for `$brand-color` and `$brand-color-dark`

---

### Updating Home Image

1. Put your new image in the folder `/img/`

2. Open `/css/main.scss` and find the line `article.home {`

3. Between the curly braces ({}) that follow, there should be a line that says `background-image: url('/img/<arbitrary_image_name>.jpg');`

4. Replace the `<arbitrary_image_name>.jpg` with the name of your new image.

---

### Updating About

1. Open the file `/about.html`.

#### Updating Text

2. Simple update the text under `<!-- CHANGE TEXT HERE -->`

#### Updating Image

2. Add your new image to `/img/`

3. Update the src property of the img tag under `<!-- CHANGE PROFILE IMAGE HERE -->` to point to that image

---

### Updating Resume

1. Upload your resume with **public** access on Google Drive

2. Follow this tutorial to get the <iframe> embed code from Google Drive: [link](http://www.alicekeeler.com/2016/06/05/google-drive-embed-pdf/)

3. Update the <iframe> tag in `/resume.html` with your newly generated one

---

### Update Portfolio

1. Open `/portfolio/index.html`

2. Note that this portfolio is organized by 3 columns, labeled by `<!-- COLUMN 1 -->`, `<!-- COLUMN 2 -->`, and `<!-- COLUMN 3 -->`

3. Adding new img html tags on the top of each column will list them at the top of the website. Adding new img html tags at the bottom of each column will do the opposite.

4. To add a new image, add your image file to `/portfolio/img` and follow this template to add new code to one of the three columns in `/portfolio/index.html`

```
<a href="#" data-featherlight="/portfolio/img/<YOUR_IMAGE_NAME>.jpg">
  <img src="/portfolio/img/<YOUR_IMAGE_NAME>.jpg" alt="">
</a>
```

---

### Writing a New Blog Post

1. Create a new file in the directory `/blog/_posts/<FILENAME>`. The new file must be named in this standard format: `2016-07-26-name-of-your-post.md`

2. Add a square shaped preview image and any other images you may want into `/blog/img/`

3. Copy paste the template file's contents (`/blog/_posts/blog/_posts/TEMPLATE.md`) into your new blog post file.

4. Edit the text that follows `title:`, `author:`, `preview_img` (with the name of the square preview image you added before), and `excerpt:`

5. Optionally edit text after `optional_top_banner_img:` and `optional_bottom_banner_img:` with the names of your banner images

6. Optionally add a gallery of images at the bottom of your blog post by editing the text that follows `optional_gallery_img_list:`. Ensure your text follows the following format:
```
['my_first_image.jpg', 'my_second_image.jpg', 'my_third_image.jpg', 'etc...']
```

7. Edit the body of your blog post by putting text under `<!-- BELOW HERE IS WHERE YOUR POST'S BODY WILL GO -->`. Wrap headings in h2 tags as shown in the template example. Leave lines between paragraphs to make them separate paragraphs.

8. Congratulations you have made a new post.

---

### Update Contact Email

1. Open `/contact.html`

2. Find the line that says `<form class="contact-form" method="POST" action="http://formspree.io/<arbitrary_email@gmail.com>"`

3. Replace `<arbitrary_email@gmail.com>` with your new email

4. Try sending a test message to yourself

---

### For Local Development Purposes:

1. Run `$ bundle exec jekyll serve` to serve the website locally at port `4000`

2. Open browser at `localhost:4000` and begin developing!
