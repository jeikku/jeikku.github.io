## How to Host a Resume on a  Static Website 
#### & The Value of Technical Writing

### **Purpose**
This README will serve to teach you the basics of modern technical writing. It will also explain how to utilize fundamental tools and walk you through the process of formatting your resume on a hosted website. This README will also make heavy reference to Andrew Etter's book [*Modern Technical Writing*](https://www.markdowntutorial.com/), as it is a great reference for current Technical Writing practices. Through the explanations given you will have gained an understanding of current technical writing practices.  
In particular, this guide will make frequent reference to three main points of technical writing. These include using a lightweight markup language; Formatting documents using a static site generator; and using a version control system for document sharing and hosting. Don't worry if these are new concepts to you, as explanations and/or [resources to learn more](https://jeikku.github.io/README/#more-resources) are provided.

### **Hosting a Resume - Requirements**
Here is the software stack which we will use:  

> Lightweight markup language: **Markdown**
	  
> Markdown Editor: **Ghostwriter**  
  
> Static Site Host: **GitHub Pages**  
  
> Static Site Generator: **Jekyll**

#### What are these anyway?
- A **lightweight markup language** is the cornerstone of modern technical writing. It offers a simplistic and highly readable layout. Depending on the language you choose, it can also have many built in formatting options. The most popular one is Markdown. You can find a tutorial on how to use it under the [*More Resources*](https://jeikku.github.io/README/#more-resources) section.  

- To write and edit your Markdown (.md) file with ease, we will also be using the **Markdown editor** [Ghostwriter](https://ghostwriter.kde.org/). There are many choices for editors; Ghostwriter in particular provides a sleek interface where you can immediately see the formatted output as you write  

- A **static site** is any website which lacks non-static components. These websites are often used for documentation, and do not require a database or any dependencies (Etter, pg. 21). GitHub Pages will provide the means to host your website.  

- To easily create a static website, we will be using the **static site generator** (or **SSG**) [Jekyll](https://jekyllrb.com/). An SSG provides resources to generate static websites, such as pre-existing themes which can be seamlessly applied. Jekyll was chosen due to its integration with GitHub Pages, making it easy to work with

Additionally, you will be required to make a **resume formatted in markdown**. A sample is provided under the [*More Resources*](https://jeikku.github.io/README/#more-resources) section. Feel free to use this as a reference.

### **The Process**
As explained in Andrew Etter's book *Modern Technical Writing*, it isn't easy to produce content that other people want to read and will find useful. Therefore, each step for creating and hosting your resume will also provide context into the practices behind it, to help better explain the process.

1. **Write your Resume in Markdown**  
- After you have completed the tutorial on Markdown syntax (link under [*More Resources*](https://jeikku.github.io/README/#more-resources)), it's time to start writing. Open up Ghostwriter. Before you start writing, however, it is important to consider stylistic choices.  
	- Etter explains that writing with consistency is one of the core aspects to readability (Etter, pg. 10). Furthermore, that consistency can be applied to clean formatting throughout your resume. Utilize lists, headers, and inline styling in order to create a resume that can be easily dissected by the eyes.

2. **Revise your Resume**  
- Now that you have written out and formatted your resume to be easily readable, it's time to go through it and ensure that it answers some fundamental questions. In the context of a resume, ask yourself if the skills and experience listed are relevant to the companies you want to apply for. In the book Etter also makes it clear that you should write out your skills based on verifiable proof, and avoid writing from memory (Etter, pg. 8-10). This is to ensure you are being concise and accurate with your statements. On a resume, for instance, you wouldn't want to write down something that can't be well explained or backed up during an interview.	

3. **Get setup with GitHub Pages**  
* It's now time to create an account on GitHub and make your static site.  
	* Once you've logged in: Click on the icon in the top right and navigate to 'Your Repositories'. Click the green 'New' button  
	* It is important that you name the repository *(username)*.github.io  
		* **Note:** replace *(username)* with your own username  
	* Enable 'Add a README file'. This is what you will use for resume later  
	* Navigate to your project repository. Click on 'Settings'. Click on 'Pages' (under the *Code and automation* tab)  
	* Under 'Branch' select 'Main'. After a few minutes your website will now be live at *your_username*.github.io !

4. **Add your formatted resume file**  
	* You can easily insert your resume .md file to the site by replacing the README.md file with it. Ensure that the resume file is also renamed to README.md, as this is what GitHub Pages will use for the website's homepage.	  
		* **Note:** The website will take around ~1 minute to update  
	- Because GitHub is a [version control](atlassian.com/git/tutorials/what-is-version-control) service, it is seamless to make safe changes to your website as you see fit, which is an incredibly valuable technical writing practice (Etter, pg. 18-19).

5. **Generate the Static Site Theme with Jekyll**  
- On top of good styling, having an eye catching and clean site for your resume will bring it to the next level. Create a file in your repo called '_config.yml', where you will set a site-wide theme and title. GitHub has some [Jekyll themes](https://pages.github.com/themes/) integrated, otherwise you can browse the web for more choices. In _config.yml, insert the following code to set the site's theme and title (replacing with your own):  

	```
	Theme: jekyll-theme-midnight
	Title: My Resume
	```

With a good looking theme and clean static site, you are now acquainted with core modern technical writing practices!

Here is an example of what your newly hosted Resume might look like:  
![samplegif](https://github.com/jeikku/jeikku.github.io/blob/main/resume.gif)

### **Frequently Asked Questions Q&A**

**Q** - How do I change my website's homepage?  
* **A** - By default GitHub Pages will recognize README.md as the homepage for your static site. However, you can include an index.md file which will overwrite README.md as the main page.  
Alternatively, you can insert the following text at the top of your preferred homepage *.md* file:  

	```
	---
	permalink: //
	---
	 ```

* What this is doing is setting the sub-URL of the page to nothing, making it the same URL as the homepage
	
**Q** - How do I write concisely?  
* **A** - This is naturally a question that is somewhat open to individual interpretation. However, basing an answer off of the rules defined in Etter's book, one of the basic strategies is to 'Define the Audience'. Regarding this topic, Etter explains that writers make much better assumptions when they know exactly who they are writing to (Etter, pg. 6-8). For example, a painter who writes an introductory guide to painting would know to write as though the audience knows nothing on the subject beforehand. Whereas' an advanced painters guide would not waste time covering basic techniques.

### More Resources
Andrew Etter's Book:  
[Modern Technical Writing](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS "Modern Technical Writing")

Markdown Tutorial:  
[markdowntutorial.com](https://www.markdowntutorial.com/ "Markdown Tutorial") 

Sample Resume (formatted in markdown):  
[jeikku.github.io](https://jeikku.github.io/ "Resume | Jacob Broggy")

Jekyll Theme Examples:  
[Jekyll Themes](https://pages.github.com/themes/ "Themes")

What is Version Control:  
[Version Control Introduction](atlassian.com/git/tutorials/what-is-version-control)
