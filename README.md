# The Woodland Wag 

Milestone Projet 1 - Dominic Foster

[Page link](https://https://domfoster1.github.io/the-woodland-wag-mp1/)

[Github link](https://github.com/domfoster1/the-woodland-wag-mp1)

## Table of Contents

1. **UX**
- Project goals

- Developer and Business goals

- User Stories

- Design choices

- Wireframes

2. **Features**

- Existing features

- Features left to implements

3. Technologies used

4. Deployments

- How to run this project locally

5. Testing

6. Credits

- Content

- Media

- Code

- Acknowledgements


## **UX** 

### **Project goals**

The primary goal of this project is to provide all neccessary information to users for 'The Woodland Wag', a pet services business located on Cannock Chase. The project is aimed at users of all ages so a simple colour palette is used with easy to read fonts so it does not discourage anyone from using the website.

### **Developer and Business goals**

The business goals of this project are to increase custom and help spread the name of the business. The developer goal is to create a clear and engaging website to help achieve the business goals. Their target audience are dog owners.

### **User stories**

**User story 1** 

I need a website that has a clear, easy to use layout and it will respond to whichever device I choose to use without becoming difficult to use.


**User Story 2**

I am a dog owner needing a business to look after my dog. I need information laid out clearly to help me decide whether this business is suitable for my job


**User story 3**

I am in need of a new dog sitter and would like to see what kind of activities my dog would get up to through photos

**User story 4**

I am a prospective customer and I would like to make an enquiry so I can start planning for the future

**User story 5**

I am a prospective customer and I would like to see the reviews of the business before deciding whether to book

### **Design Choices**

The users of the website could be any age from 18 +, that are leaving theirs dogs in the hands of a stranger which can be a very stressful experience. The following choices were made with that in mind:

1. Simple and efficient layout - in keeping with best practices (Navbar, footer on each page)
2. Engaging pictures from the start
3. Neuteral and calming colors
4. Primary and secondary colors chosen as the business is called "The **Woodland** Wag" so it relates to the leaves and trees

|Primary font|Nunito/sans-serif| 
|Secondary font| Funnel Sans / sans-serif|
| Primary Color  | #4b5a3c  |   
| Secondary Color  | #3a2620  |
| Light Highlight Color | #f3e1c6 |

The Fonts chosen were specifically chosen as this project is aimed at all ages so it was necessary to have easy to read fonts.


### **Wireframes**

Here is a link to the wireframes I created for this project

https://balsamiq.cloud/s55wkp9/pspea63



## **Features**

### Navbar

The navigation bar has been fixed to the top of the page so it is always available to the user and also does not cover up any of the main content. The Navbar is responsive and creates a drop down menu for smaller screens whilst keeping the logo and company name.

### Hero image

The hero image is there so the user gets an immediate feel for the company and what it is all about (Dogs out exploring woodlands).


### Carousel

The carousel has been included next to the about me section to show more photos of the services to the user whilst they are browsing the website. It has an automatic function so the user does not have to manually move it but they are able to scroll back and forth if they would like to.

### Service Cards

I included service cards as I believe this to be a tidy and efficient way to show the services of the company. They line up in a row on desktop and then sit on top of one another on tablets and smaller screens.

### Location page

I created a seperate location page which shows where the company is based and the surrounding area. I thought it was important to use a bigger map rather than a small one (in a footer for example) as the customer needs to know how close the company is to them. It also shows off how close the company is to Cannock chase, which may encourage them to use the company more.

### Enquiry form

I created an Enquiry form page which you access through buttons in the Navbar and footer on every single page. The enquiry form has a requirement on all options other than the text area so none are missing. Dropdown and radios are used to make the information as clear and concise as possible for both the company and the user.

### Footer

The footer appears on each page and contains

- links to both Facebook and instagram
- the logo
- comapny name
- email address
- phone number
- button to enquiry page

I did this for both the continuity aspect and as it is a standard procedure that the user would expect.

### Features left to implement

I was unable to add the reviews section. This is a feature that I didn't feel was necessary but would be a nice inclusion at a later date.



## Technologies used

### Languages

I used HTML and CSS to complete the project

### Programs

I used Visual Studio Code to write the code and GitHub as a repository and to deploy. 



## Deployments

First of all I created a repository on Github and then copied the following into my repository on Visual studio Code:

- git config --global user.name
- git config --global user.email
- git config --list

The project was developed of Visual studio Code then commited and pushed to GitHub using the following steps:

- git add . 
- git commit -m "Information about changes"
- git push 

I did not push the commits every single time I commited, however tended to do this after 4 commits.

After completing the majority of the project, I then set it for deployment. To do this I did the following from my repository:

- Went to Settings > Pages
- Ensured "Deploy from a branch" was chosen
- Chose the main branch
- clicked save
- waited for deployed site

## Testing

### Devices

**Ipad and iPhone 11** 

Everything works as expected, nav bar dropdown opens and closes and all pages formatted correctly

**Samsung A53** 

Everything works as expected, nav bar dropdown opens and closes and all pages formatted correctly

**Laptop L screen** 

Everything works as expected, nav bar dropdown opens and closes and all pages formatted correctly

**Laptop XL screen**

Everything works as expected, nav bar dropdown opens and closes and all pages formatted correctly

### Bugs throughout the process

During the process I encountered a few issues that I had to to resolve

- Footer on succes.html not sticking to the bottom, I resolved this using the following styles

html, body {
  height: 100%;
  margin: 0;
}

.wrapper {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

main {
  flex-grow: 1;
}

- The navbar and footer width reduced on the location.html, I realised this was because the map was enlarging the page. I corrected this by creating the following media query

/*Media queries for small and larger mobiles*/

@media screen and (max-width:425px) {
  #map {
    max-width: fit-content;
  }
}

### W3 HTML Validator 

I have used the W3 html validator to check over all the pages of the project to correct any issues in the code. It found the following issues :

- I applied width to the "enquiry" buttons. This was a unnecessary addition as it didn't effect the buttons in anyway so I removed it.

- I wrapped the buttons in <a> element. Whilst this worked visually it was not valid html coding. I corrected this by using 

<a href="enquiry.html" class="btn btn-outline-primary custom-button-outline" role="button">Make an Enquiry!</a>

- There were several elements that were not closed off throughout the pages, I have since closed off all the necessary elements

I corrected all mistakes found by the validator and it is now free of mistakes

### W3 CSS Validator

I used the W3 CSS validator and it found no mistakes

### Lighthouse 

I used lighthouse to test the performance, accessibility and best practices of the site. 

The performance on my Laptop was coming out at 75% as it is quite a low performing laptop. However testing on a higher performance laptop it came out at 90%. Initially this was much lower, I then converted all my images to webp and it was much improved.

The accessibility performance of the page is 98%

The best practice performance of the page is 100%

## Credits

### Content

All of the text was written myself

### Media

I got the favicon from https://icons8.com/icons/set/dog

The hero image was sourced from https://www.pexels.com/photo/english-cocker-spaniel-puppy-sitting-on-ground-beside-grass-1254140/

The logo was created by using ChatGPT

All other images were taken by myself

### Code

I used Bootstrap for the carousel (https://getbootstrap.com/docs/4.0/components/carousel/#with-controls)

Navbar https://getbootstrap.com/docs/4.0/components/navbar/

and also for the service cards (https://getbootstrap.com/docs/4.0/components/card/)














 







