# Project IC People - Student Pages

## Introduction:

The goal of this project is to offer Master and grad students from IC School with an EPFL domain webpage where they can showcase information about themselves and their research.

Keep in mind that :
* Each user has a quota of 1Gb
* After your departure from EPFL, there will be a grace period of 6 months

## Objectives:

The main objectives of this project: <br />
* Provide an easy and ready to use template for Master and grad students,
* Uniformize the webpages with EPFL graphical elements,
* Provide a modular based page with CSS/JS/html that can be customized and adapted as needed.

## Page structure:

### 1. Main structure

The code is divided into three  parts: <br />
* The main HTML file (index.html) --> simple to modify<br />
* Three examples files (examples folder) --> you can take inspiration from them<br />
* The “css/blocks (CSS stylesheets) --> can be modified to add your style modifications<br />
* The “css/fixed” CSS files that makes the visual unity and integrity of the project --> **do not modify**
### 2. Blocks

There are currently 8 blocks in html :

* **About:** <br />
  Write a short (for a better visual result, between 100 and 170 words) description about yourself, your experience and anything you’d like to highlight.
* **Assocations:** <br />
  If you've ever been in a student assocation, add it into this block.
* **Awards:** <br />
  Here you can add your achievements or awards.
* **Career summary:** <br />
  Here you can add your career path and academic experience.
* **Press coverage:** <br />
  Here you can add any media coverage you’ve had with links to magazines, websites, etc.,
* **Projects:** <br />
  Here you can add the projects you’ve been working on.
* **Recent publications:** <br />
  Is a highlight of your two most recent publications and a poster.
* **Publications:** <br />
  Here you can add your publications.
## Styles
* If you need to add a element, you can use the general
[styleguide of EPFL](https://epfl-si.github.io/elements/#/) as a guide.
* Otherwise you can create a css file in the "css/blocks" folder to do your changes, and link this into the "head" of index.html
## Getting started

#### 1. Setup

For hosting the files, we use an SFTP server. You have to be connected to EPFL VPN (https://www.epfl.ch/campus/services/ressources-informatiques/network-services-reseau/acces-intranet-a-distance/clients-vpn-disponibles/).
Access infos <br />
Host: icvm0047.xaas.epfl.ch <br />
Username: Gaspar Username <br />
Password: Gaspar Password <br />
index folder: public_html <br />

Copy and paste all the files from IC mypage-test-template into the public_html folder (examples folder and README are optional).

If you don't know how to acess an SFTP server, here is two tutorials.
##### 1.1 Windows/MacOS

1. Go to https://cyberduck.io/download/

2. Download and install it

3. Go on the application and click on the button circled in red on the image. Once in this menu press the + at the bottom left

<img src="https://user-images.githubusercontent.com/45627872/121321032-083ef180-c90e-11eb-8a45-ab0f3c7bb348.png" width="750"/>

4. At the top click on SFTP

5. In the server field enter: icvm0047.xaas.epfl.ch

6. For the field username and password: use your GasparAccount. 

![image](https://user-images.githubusercontent.com/45627872/117404521-5aa18280-af0a-11eb-9bd2-b8f395b06322.png)

7. Next, close the window

8. Double click on the connection and click on allow

9. Double click on public_html

10. Here you can place your files

11. Your site will be accessible on the following URL: https://mypage-test.epfl.ch/~GasparAccount

##### 1.2 Linux

1. Connect to the EPFL VPN

2. Use ``` sftp GasparAccount@icvm0047.xaas.epfl.ch ```

3. Enter your Gaspar password

4. Get into public_html dir with ``` cd public_html ```

5. Use ``` put myFile ``` to put your files in your directory

6. Your site will be accessible on the following URL: https://mypage-test.epfl.ch/~GasparAccount

7. That's it!

#### 2. Creating your page

Note: Everything in Italic and behind * should be replaced.
For the layout, we used bootstrap. You can add a grid by adding the col- classes. More information on https://getbootstrap.com/docs/4.0/layout/grid/.
Feel free to delete or add blocks as you want - this is the point of having modular blocks.

#### **1. Some cool HTML/CSS/JS Editors**

1. Atom 
   Cool IDE, devlopped by GitHub team, open source.
2. VSCode
   Light, lots of extensions.
3. Notepad
   Light, available on every windows machines. Good Luck.


#### **2. Fixed blocks - Header, footer, about**

Here is a step-by-step tutorial on how to fill basic information on the html file.

* In the `<head>`, change the `<title>` tag to your name : e.g. `<title>`*Mathis Sandoz*`</title>`
* In the `<body>`
    * a. Add your profile picture: change the `<img src="img\fixed\*myPhoto.png*" id="profilPicture">`
    * b. Change `<h2>Samuel Hayden</h2>` change *Samuel Hayden* by your name.
    * c. Add your title and lab: change the `<strong>` *mytitle* `</strong>`, the `<a target="_blank" href=*https://mylab.epfl.ch>*` *my lab* `</a>`. If you don't have a lab, delete the <a></a> tag.
    * d. Add your contact information. If you don't have one of them, delete it:
         Email --> `<a href="mailto:*my.name*@epfl.ch">` *My name* `</a>`<br />
         Tel --> `<a href="tel:+41791234567">`*+41 79 123 45 67*`</a>`<br />
         Office location --> `<a href="*https://plan.epfl.ch/?room==BC%20402*">`*BC 402*`</a>`<br />
         Postal address --> `<a href="*https://mylab.epfl.ch/contact*">EPFL, IC, *mylab*,`<wbr>` *Station 14* `<br>` CH 1015 Lausanne `<wbr>` Switzerland`</a>`
* In the `<footer>`
    Change your info :
    `<p>` *myname* | `<a class="footerLinks" href="mailto:*my.name@epfl.ch*">`my.name@epfl.ch`</a>` | `<a class="footerLinks" href="*https://plan.epfl.ch/?room==BC%20402*">`*BC 402*`</a>` | *Mylab*`</p>`
* In the `<div class="about">`, Write a short description, for a better visual result, between 100 and 170 words about yourself, your experience and anything you’d like to highlight.

```
<div class="about">
    <h3>
        About
    </h3>
    <p>
        some lines about you, your experiences and everything you want
    </p>
</div>
```

#### **3. Modular blocks**<br />

You can delete, add or modify blocks as you like, as long as they respect the graphic guidelines.

#### Recent publications<br />
This block is a spotlight for your two latest publications, the rest will appear in the "publications-more" block.

```
<div class="publications-recent">
  <h3>Recent Publications</h3>
  <div class="col-6">
    <a href="#mylastPublication">
      <img class="img-responsive" src="myimage.jpg">
      <h5>Highlight 1</h5>
      <p>A short description of your publication</p>
    </a>
  </div>
  <div class="col-6">
    <a href="#mySecondlastPublication">
      <img class="img-responsive" src="myimage-2.jpg">
      <h5>Highlight 2</h5>
      <p>A short description of your publication</p>
    </a>
  </div> <a href="#publications-more">More publications... ></a>
</div>
```

![1](https://user-images.githubusercontent.com/78591401/116852713-1ace5880-abf5-11eb-935d-9256b94a0054.png)


#### Assocations <br />
Here you can add the assocations you've been involved into.

``` 
<div class="associations col-md-3">
  <h3>Associations</h3>
    <div class="associations-child">
      <input id="assoc-1" type="radio" name="tabs">
      <label for="assoc-1" ><img src="https://clic.epfl.ch/img/logo.png"><span>2021 - now<br>Coach, CLIC EPFL</span></label>
      <div class="assoc-content">
        <p>The CLIC is the Computer Science and Communications Student Association of the École Polytechnique Fédérale de Lausanne (EPFL). <br> During my time at the CLIC I was in charge of the following tasks : <br></p>
        <ul><li>Lorem ipsum dolor sit amet.</li><li>Lorem ipsum dolor sit amet.</li><li>Lorem ipsum dolor sit amet.</li><li>Lorem ipsum dolor sit amet.</li></ul>
      </div>
    </div>
    <div class="associations-child">
      <input id="assoc-2" type="radio" name="tabs">
      <label for="assoc-2"><img src="https://agepoly.ch/wp-content/themes/agepoly/resources/Horizontal_-_AI_-_AGEPoly.svg"><span>2019 - 2020<br>President, AGEPoly EPFL</span></label>
      <div class="assoc-content">
        <p>AgePoly is the student association of the EPFL.</p>
        <ul><li>Lorem ipsum dolor sit amet.</li><li>Lorem ipsum dolor sit amet.</li><li>Lorem ipsum dolor sit amet.</li><li>Lorem ipsum dolor sit amet.</li></ul>
      </div>
    </div>
    <div class="associations-child">
      <input id="assoc-3" type="radio" name="tabs">
      <label for="assoc-3"><img src="https://clic.epfl.ch/img/logo.png"><span>2021 - now<br>Coach, CLIC EPFL</span></label>
      <div class="assoc-content">
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ac laoreet elit. Phasellus dignissim purus vitae urna cursus, quis congue ligula tristique. Ut nec blandit risus. Donec at orci ut justo venenatis viverra.</p>
        <ul><li>Lorem ipsum dolor sit amet.</li><li>Lorem ipsum dolor sit amet.</li><li>Lorem ipsum dolor sit amet.</li><li>Lorem ipsum dolor sit amet.</li></ul>
      </div>
    </div>
    <div class="associations-child">
      <input id="assoc-4" type="radio" name="tabs">
      <label for="assoc-4"><img src="https://clic.epfl.ch/img/logo.png"><span>2021 - now<br>Coach, CLIC EPFL</span></label>
      <div class="assoc-content">
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ac laoreet elit. Phasellus dignissim purus vitae urna cursus, quis congue ligula tristique. Ut nec blandit risus. Donec at orci ut justo venenatis viverra.</p>
        <ul><li>Lorem ipsum dolor sit amet.</li><li>Lorem ipsum dolor sit amet.</li><li>Lorem ipsum dolor sit amet.</li><li>Lorem ipsum dolor sit amet.</li></ul>
      </div>
    </div>
</div>a
 ``` 

![image](https://user-images.githubusercontent.com/45627872/122885658-9029f000-d33f-11eb-9018-824d63bb9cb8.png)

#### Awards<br />

Here you can add your achievements or awards.

```
<div class="awards">
  <h3>Awards</h3>
  <ul>
    <li>Award 1</li>
    <li>Award 2</li>
    <li>Award 3</li>
    <li>Award 4</li>
  </ul>
</div>
```

![2](https://user-images.githubusercontent.com/78591401/116852736-26ba1a80-abf5-11eb-9ea2-ce112c682d23.png)

#### Press coverage<br />
Here you can add the magazines or newspaper you/your work appeared in.

````
<div class="press-coverage">
  <h3>Press coverages</h3>
  <a target="_blank" href="https://www.aMagazine.com">
    <img class="img-responsive" src="logoMagazine.jpg”>
  </a>
  <a target="_blank" href="https://www.aMagazine.com">
    <img class="img-responsive" src="logoMagazine.jpg”>
  </a>
  <a target="_blank" href="https://www.aMagazine.com">
    <img class="img-responsive" src="logoMagazine.jpg”>
  </a>
  <a target="_blank" href="https://www.aMagazine.com">
    <img class="img-responsive" src="logoMagazine.jpg”>
  </a>
</div>
````

![3](https://user-images.githubusercontent.com/78591401/116852824-523d0500-abf5-11eb-995c-530235bd225b.png)


#### Career

This block is separated in two parts: the timeline and the biography. Feel free to keep both or delete one of the two.

````
<div class="career">
    <h3>Career</h3>
    <div class="timeline">
        <div>
            <img class="logo-carrer" src="myFirstUniversityLogo.jpg">
            <button data-toggle="collapse" data-target="#career1">2008 – 2011 v</button>
            <div id="career1" class="collapse">Name of the university, what I did in here, …</div>
        </div>
        <div class="inBetween"></div>
        <div>
            <img class="logo-carrer" src="mySecondUniversityLogo.jpg ">
            <button data-toggle="collapse" data-target="#career2">2011 - 2016 v</button>
            <div id="career2" class="collapse">Name of the university, what I did in here, …</div>
        </div>
        <div class="inBetween"></div>
        <div>
            <img class="logo-carrer" src="myThirdUniversityLogo.jpg">
            <button data-toggle="collapse" data-target="#career3">2016 - 2017 v</button>
            <div id="career3" class="collapse">Name of the university, what I did in here, …</div>
        </div>
        <div class="inBetween"></div>
        <div style="margin-left: -15px;">
            <img class="logo-carrer" src="myFourthUniversityLogo.jpg">
            <button data-toggle="collapse" data-target="#career4">2017 - Now v</button>
            <div id="career4" class="collapse"> Name of the university, what I did in here, …</div>
        </div>
    </div>
    <p>Some lines about your career</p>
</div>
````

![7](https://user-images.githubusercontent.com/78591401/116852944-84e6fd80-abf5-11eb-8065-5f3e7a186572.png)

#### Projects

A space where you can showcase your research.

You can use three different formats:

* Projects with a picture

```
<div class="projects">
    <h3>Projects</h3>
    <a target="_blank" href="https://myProjectWebsite.com">
        <div class="col-md-6">
        <img class="img-responsive" src="myProjectPic.jpg (best result will be with a square image)">
        <h5>Project 1</h5>
        <p>A short description of the project.</p>
        </div>
    </a>
    <a>
        <div class="col-md-6">
        <img class="img-responsive" src="myProjectPic.jpg (best result will be with a square image)">
        <h5>Project 2</h5>
        <p>A short description of the project.</p>
        </div>
    </a>
    <a target="_blank" href="https://myProjectWebsite.com">
        <div class="col-md-6">
        <img class="img-responsive" src="myProjectPic.jpg (best result will be with a square image)">
        <h5>Project 3</h5>
        <p>A short description of the project.</p>
        </div>
    </a>
    <a target="_blank" href="https://myProjectWebsite.com">
        <div class="col-md-6">
        <img class="img-responsive" src="myProjectPic.jpg (best result will be with a square image)">
        <h5>Project 4</h5>
        <p>A short description of the project.</p>
        </div>
    </a>
</div>
```

![4](https://user-images.githubusercontent.com/78591401/116852853-5e28c700-abf5-11eb-9f2b-e1b5b20bd28c.png)

* Projects with a long description

In this style, you can add a longer description and more projects due to the pagination.

The recommended number of projects by page is 2 or 3. To add more pages you have to add:

````
<ul id=”pro-pageNumber”>My page content</ul>
````

And at the end, in the nav-pub-buttons div:

````
<button id="nav-pro-btn-pageNumber" onclick="navPropageNumber()">pageNumber</button>
````

You’ll have to change the ID of the inputs and the FOR of the labels for every project you add:

````
<input type="checkbox" class="read-more-state" id="downMore-myProjectNumber" /> and label for="downMore-myProjectNumber" class="read-more-trigger"></label>
````

````
<div class="col-md-5 projects">
    <h3>Projects</h3>
    <ul id="pro-1">
        <li>
            <a target="_blank" href="https://www.myProjectWebsite.com">
                <h5>Project 1</h5>
                <p>Short description e.g. people who worked on it.</p>
            </a>
            <input type="checkbox" class="read-more-state" id="downMore-1" />
            <p class="read-more">A long project description.</p>
            <label for="downMore-1" class="read-more-trigger"></label>
        </li>
        <li>
            <a target="_blank" href="https://www.myProjectWebsite.com">
                <h5>Project 2</h5>
                <p>Short description e.g. people who worked on it </p>
            </a>
            <input type="checkbox" class="read-more-state" id="downMore-2" />
            <p class="read-more">A long project description.</p>
            <label for="downMore-2" class="read-more-trigger"></label>
        </li>
    </ul>
    <ul id="pro-2">
        <li>
            <a target="_blank" href="https://www.myProjectWebsite.com">
                <h5>Project 3</h5>
                <p>Short description e.g. people who worked on it.</p>
            </a>
            <input type="checkbox" class="read-more-state" id="downMore-3" />
            <p class="read-more"> A long project description.</p>
            <label for="downMore-3" class="read-more-trigger"></label>
        </li>
        <li>
            <a target="_blank" href="https://www.myProjectWebsite.com">
                <h5>Project 4</h5>
                <p>Short description e.g. people who worked on it.</p>
            </a>
            <input type="checkbox" class="read-more-state" id="downMore-4" />
            <p class="read-more">A long project description.</p>
            <label for="downMore-4" class="read-more-trigger"></label>
        </li>
    </ul>
    <div id="nav-pub-buttons">
        <button id="nav-pro-btn-1" onclick="navPro1()">1</button>
        <button id="nav-pro-btn-2" onclick="navPro2()">2</button>
    </div>
</div>
````

![5](https://user-images.githubusercontent.com/78591401/116852899-726cc400-abf5-11eb-9ecc-461748e820b1.png)

* Projects with a simple list

````
<div class="col-md-3 projects">
    <h3>Projects</h3>
    <ul>
        <a target="_blank" href="https://www.myProjectWebsite.com">
            <li>
                <h5>Name of the project and a simple description</h5>
            </li>
        </a>
        <a target="_blank" href="https://www.myProjectWebsite.com">
            <li>
                <h5>Name of the project and a simple description</h5>
            </li>
        </a>
        <a target="_blank" href="https://www.myProjectWebsite.com">
            <li>
                <h5>Name of the project and a simple description</h5>
            </li>
        </a>
    </ul>
</div>
````

![6](https://user-images.githubusercontent.com/78591401/116852916-7ac4ff00-abf5-11eb-9836-539cf54a7375.png)


#### Publications

````
<div class="publications-more col-md-4" id="publications-more">
    <h3>Publications</h3>
    <ul id="pub-1">
        <li>
            <a href="#popup1">
                <!-- in order to make more popups, you need to change the href "#popup1" to "#popup2" for the second, "#popup3" for the third, ...-->
                <div class="ctn-img">
                    <img src="myPublicationImg.jpg" />
                </div>
                <h5>Publication name</h5>
                <!-- Here is the name of your publication-->
                <p>A short description of this publication</p>
            </a>
            <div id="popup1" class="overlay popup">
                <!-- You need to change the id "popup1" to "popup2" for the second, "popup3" for the third, ... here as well-->
                <div class="content"> <a class="close" href="#section">&times;</a>
                    <h1 id="popupH2">Publication Name</h1>
                    <div class="buttons-publications">
                        <button type="button">
                            <a target="_blank" href="myPaper.pdf"> You can add here a link to the paper in PDF, additionnal informations, videos, ...</a>
                        </button>
                        <button type="button">
                            <a target="_blank" href="https://www.myVideo.ch"> You can add here a link to the paper in PDF, additionnal informations, videos, ...</a>
                        </button>
                        <button type="button">
                            <a target="_blank" href="https://www.myLabwebsite.ch"> You can add here a link to the paper in PDF, additionnal informations, videos, ...</a>
                        </button>
                    </div>
                    <p><strong>Abstract</strong>
                        <br>Publication here (you can add whatever you want : img, vids, text, …
                    </p>
                </div>
            </div>
        </li>
        <li class="publications-li-less">
            <a target="_blank" href="publication.pdf">
                <h5>Publication title</h5>
                <p>A short description</p>
            </a>
        </li>
    </ul>
    <ul id="pub-2">
        <li class="publications-li-less">
            <a target="_blank" href="publication.pdf">
                <h5>Publication title</h5>
                <p>A short description</p>
            </a>
        </li>
    </ul>
    <div id="nav-pub-buttons">
        <button id="nav-pub-btn-1" onclick="navDiv1()">1</button>
        <button id="nav-pub-btn-2" onclick="navDiv2()">2</button>
    </div>
</div>
````

![Publications2](https://user-images.githubusercontent.com/70935737/114377006-770a0380-9b86-11eb-8122-e47143ac640c.png)


Pop up:

![Picture 6](https://user-images.githubusercontent.com/78591401/113692995-68c36f80-96ce-11eb-9183-11325b28d595.png)

#### Graphic guidelines

##### Generalities

The graphic guidelines follow the EPFL guidelines. It ensures that the pages remain coherent.

##### Colors

- Black ![#000000](https://via.placeholder.com/15/000000/000000?text=+) `#000000`
- Pearl Grey ![#E5E5E5](https://via.placeholder.com/15/E5E5E5/000000?text=+) `#E5E5E5`
- Red ![#FF0000](https://via.placeholder.com/15/FF0000/000000?text=+) `#FF0000`
- Violet ![#5C2483](https://via.placeholder.com/15/5C2483/000000?text=+) `#5C2483`

##### Font & paragraphs

The font to use is arial. For a better UX, maximum 70-90 characters per line (10-15 words).

##### Margins

The page must be in full size with no margins.

##### Multipage

The website must have only one page.

##### Images

Pixel density of the images must be at least 72dpi.
