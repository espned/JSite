# JSite - Website software based on pure HTML, CSS, JavaScript and JSON
This is the website code based on pure HTML,CSS, JavaScript and JSON. This code is useful for developing websites who write tutorials, articles, documentation. Simple configuration steps to setup the site and easy to write articles/tutorials for your website. 

![alt HTML, CSS, JavaScript, JSON](https://img.shields.io/badge/Technologies-HTML,%20CSS,%20JavaScript,%20JSON-deeppink?style=for-the-badge) ![alt Vesrion 0.1](https://img.shields.io/badge/Version-0.1-green?style=for-the-badge)

# JSite Logo
![alt JSite Logo](https://drive.google.com/uc?id=1wMImMV9X9bxzEW3s18H716W3_ImShwQc&export=download)
## Alternative Logo
![alt JSite Logo](https://drive.google.com/uc?id=1WQo5FDiLfUyPoz89eLwqYpEFL3IvWD8A&export=download)


##### Color Codes of JSite Logo: White , #000000 (Black)  and #f6bb25 (Orange) 
#### Font Style of Jsite: Barlo Black
#### Letter Space : 99
#### Ltter J font size: 150
#### The word Site font size : 118
#### The word Website software font size: 25
#### Base width of the logo 500px ( based on these width the above units mentioned )

# JSite Sample Page
![alt Home Page of Jsite](https://drive.google.com/uc?id=1LimXSW54PTOtfxcWhWNXNIs6ldr2OaMk)

# Home Page of Jsite
![alt Home Page of Jsite](https://drive.google.com/uc?id=1tGtYqV7jUVXkgOl1t10PTd9XnwZh7nPO)
# Article/Tutotials Full View Page 
![alt Home Page of Jsite](https://drive.google.com/uc?id=1JKGSFYPGueScVzW1n1jxlsViNmBc6m3K)
# Code Block in Article/Tutotials Full View Page 
![alt Home Page of Jsite](https://drive.google.com/uc?id=1C1F7ZQPMX9bQil1J7BBfllA9ZRFG7nfd)
# Mobile View of Home Page
![alt Home Page of Jsite](https://drive.google.com/uc?id=1Ighk3XZUneYXLZKBdsFmK5LGH1hh6Nmu)
# How to write Articles
### images auto caption and lazy loading

```HTML
<figure class="figure">
    <img class="lazy" data-src="https://source.unsplash.com/random/642" />
    <figcaption>Image Caption Here</figcaption>
  </figure>
 ```
 
 #### images with preloader when using lazy loading concept
 ```HTML
  <figure class="figure">
    <img class="lazy" src="images/image-pre-loader.gif" data-src="https://drive.google.com/uc?id=1tGtYqV7jUVXkgOl1t10PTd9XnwZh7nPO&export=download" />
    <figcaption>Home Page of JSite</figcaption>
  </figure>
```
#### image in the right side of the content
```HTML
  <figure class="figure figure-right">
    <img class="lazy" src="images/image-pre-loader.gif" data-src="https://drive.google.com/uc?id=1wMImMV9X9bxzEW3s18H716W3_ImShwQc" />
    <figcaption>JSite Logo</figcaption>
  </figure>
```

#### image in the left side the contnet
```HTML
  <figure class="figure figure-right">
    <img class="lazy" src="images/image-pre-loader.gif" data-src="https://drive.google.com/uc?id=1wMImMV9X9bxzEW3s18H716W3_ImShwQc" />
    <figcaption>JSite Logo</figcaption>
  </figure>
```


 ### Code Blocks in Article
 Following is the snippet to add code from github repositories into article full view
 ```HTML
  <div class="codeBlock" owner="jai43" repo="spring-example-snippets" ref="master" embeded='{"path": "springBoot/@Bean/singleton_bean.java" },{"path": "springBoot/@Bean/prototye_bean.java" }' style="height:600px;"></div>
```
- **owner** attribute holds the owner of github reposiotry.
- **rep** attribute holds the name of github repository from which code to be displayed.
- **ref** attribute holds the branch name 
- **path** holds the path of the code file to be displayed in codeblock
#### example code block
[Click Here to see sample code block](#code-block-in-articletutotials-full-view-page)

## using Atom Editor 
### Snippets of JSite
To use JSite easily try to use snippets of Atom
Atom Editor is one of the best coding editor in the world. Following are the snippets of Atom for JSite 
```HTML
    '.html.text':
      # snippet 1
      'Code BLock Division':
        'prefix': 'cbd'
        'body': """<div class="codeBlock"
         owner="jai43"
         repo="${1:spring-example-snippets}"
         ref="master"
         embeded='{"path": "springBoot/pom.xml" },{"path":"springFramework/pom.xml"}'
         style="height:400px;"></div>"""
      # snippet 2
      'Content Highlitheg block':
        'prefix': 'cb'
        'body': '<cb>$1</cb>'
      # Snippet 3
      'Topic Title':
        'prefix': 'tt'
        'body': """
        <h2 class="topic_title">$1</h2>
        """
     # snippet 4
      'figure with lazy load':
        'prefix': 'fl'
        'body': """
        <figure class="figure">
         <img class="lazy" src="images/image-pre-loader.gif" data-src="${1:imageurl}" />
         <figcaption>${2:Caption of the image}</figcaption>
       </figure>
       """
     # snippet 5
      'embed video':
        'prefix': 'ev'
        'body': """

        <figure class="figure figure_video">
          <div class="videoWrapper">
            <iframe width="560" height="349" src="${1:Video URL}" frameborder="0" allowfullscreen=""></iframe>
          </div>
          <figcaption>${2:Add Video Caption Here }</figcaption>
        </figure>
        """
     # snippet 6
      'Quotes of Jsite':
        'prefix': 'quotes'
        'body': """
          <div class="quotes">
          <p>${1:Add descprtion here}
           <span class="topic">${2:Add topic name here}</span>
          </p>
        </div>
        """
     # snippet 7
      'Order List BigNumber':
        'prefix': 'olb'
        'body': """
        <div class="orderList bigNumber">
          <h3>${1:List Title or caption here}</h3>
          <ol>
            <li>
              <p class="text">${2:info1}</p>
            </li>
            <li>
              <p class="text">${3:info2}</p>
            </li>
            <li><p class="text">${4:info3}</p>
            </li>
          </ol>
          </div>
        """
    # snippet 8
      'Order List mediumSizeNumber':
        'prefix': 'olm'
        'body': """
      <div class="orderList mediumSizeNumber">
        <h3>${1:List Title or caption here}</h3>
        <ol>
         <li>
         <p class="text">${2:info1}</p>
         </li>
         <li>
         <p class="text">${3:info2}</p>
         </li>
         <li><p class="text">${4:info3}</p>
         </li>
        </ol>
      </div>
   """
```


Copy the above custom snippets into your Atom Snippet file.

##### cbd+tab 
for loading Coding block div into your article
##### cb+tab
for loading content highlight tag
##### tt+tab
for loading Topic title tag
##### fl+tab
for loading image/figure block with lazyload feature
##### ev+tab 
for loading video embeding div into your html page
##### quotes+tab
for loading quotes snippet tempaate into  current location  on the current working html page 
##### olb+tab
for loading order list with big size numbering 
#### olm+tab 
for laoding order list with medium size numbering

# Themes
JSite is flexible to adjust the feel and look of the site with theme activation.

There are three themes aditional to core theme
1) moon
2) logo
3) bold

you can change the theme in config.js file






  
  

