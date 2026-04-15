Project 1: Personal Website

The goal for this project was to create and deploy a personal website that showcases my technical abilities, houses a portfolio of projects, and serves others as a means of connecting with me. Below will contain my process, from the adaptation of a template to the deployment on Amazon Web Services. dylanhite.com

![Finished Homepage](screenshots/screenpic01.png)
Finished homepage

The first thing I did was find a template that I would be adapting. I wanted something professional with good animations, and https://html5up.net/dimension
 was the perfect match. I downloaded the template and got to work. The two files that I would be utilizing the most were index.html and main.css.

Any changes I wanted to the text and format would be done in index.html. Positioning, styling, and coloring would be done inside main.css. The process was simple: I would pick the website section I wanted to work on, find the block in the HTML, and adjust it with my own information. Easy enough for the ‘home’ and ‘about’ pages, but I had something else in mind for the ‘resume’ and ‘contact’ sections.

At the moment, I was editing the index with Notepad, because I was too lazy to download VS Code.

![Alt Text](screenshots/homepagehtml.png)

When I wanted to change or add an image, I would just drop the new picture into the images folder and call its name in the HTML function. My goal was to get a working static webpage first before making any major changes in CSS, so the individual pages were simple and mostly just lists or blocks of text. No formatting, positioning, or cursor changes yet.

Then I decided I wanted another page, totaling six. To complete this, I added:

<li><a href="#achievements">Recognition</a></li>

to the navigation pane. Then I created a new block under resume, called the article id, and added the new HTML code.

Any time I needed a large chunk of code, or if the HTML/CSS changes were complex, I co-created the code using ChatGPT.

By this point, I had a working skeleton of a webpage, but I wanted a few changes for the look to stand out:

My about page should have a side panel highlighting important points, allowing recruiters to skim
My resume page should have a clickable button to download or view my resume
I want the actual badges/images for my core certifications displayed on the recognition page
A grid for my projects; later these should be clickable to see the full project
The contact page should have working buttons that link to my other pages

Here are the changes I made for the resume page, for example:

![Alt Text](screenshots/screenpic12htmlresumeex.png)

To achieve this, I copied my resume Dylan_Hite_26.pdf and placed it under a new folder titled files. It’s on the same level as index.html, so that it can be called and used as:

files/Dylan_Hite_26.pdf

Some more visually impressive changes I made were in the recognition page. Here’s how the page turned out, followed by a block of the CSS:

![Alt Text](screenshots/screenpic04.png)
![Alt Text](screenshots/screenpic10certcards.png)

My completed code can be seen in this repository under:

cloud/personal-website/site/index.html  
cloud/personal-website/site/assets/css/main.css  
🚀 Deployment (AWS)

Now it was time to deploy my static webpage in AWS.

The first thing I needed to do was create an S3 bucket. I configured it to allow public access, uploaded my files, and enabled static website hosting. This allowed the bucket to serve my index.html file as a live website.

![Alt Text](screenshots/screenpic16.png)
![Alt Text](screenshots/bucketupload.png)
![Alt Text](screenshots/screenpic15bucketpolicy.png)

Next, I wanted to improve the project by adding HTTPS, connecting a custom domain from Route 53, and using CloudFront for better performance and security.

To do this, I:

Created a CloudFront distribution and linked it to my S3 bucket
Requested an SSL certificate using AWS Certificate Manager (ACM)
Validated the certificate using DNS validation in Route 53
Purchased a custom domain and configured DNS records
Pointed the domain to the CloudFront distribution

![Alt Text](screenshots/cdn.png)
![Alt Text](screenshots/purchaseddomain.png)

Once everything was configured, I connected all components together:

S3 → stores and serves website files
CloudFront → distributes content globally with caching
ACM → provides HTTPS encryption
Route 53 → routes domain traffic to CloudFront

![Alt Text](screenshots/finalcomplete.png)