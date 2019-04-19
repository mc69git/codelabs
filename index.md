## CodeLabs GitHub Pages

author:            Mehdi Chou.
summary:           CodeLab Tool
id:                codelab
categories:        tools
environments:      dev
status:            tutorial
feedback link:     github.com/mc69git

# Codelabs command line tool

The program takes an input in form of a resource location,
which can either be a Google Doc ID, local file path or an arbitrary URL.
It then converts the input into a codelab format, HTML by default.

For more info run `claat help`.

## Install
Duration: 0:05

The easiest way is to download pre-compiled binary.
The binaries, as well as their checksums are available at the
[Releases page](https://github.com/googlecodelabs/tools/releases/latest).

Alternatively, if you have [Go installed](https://golang.org/doc/install):

    go get github.com/googlecodelabs/tools/claat



## Create Tutorial!
Duration: 0:10

Create a file: doc.md and open this file in favorite editor.

look at [stackedit!](https://stackedit.io/app)
..and [markdown tuto!](https://www.markdowntutorial.com/)

Some basic information about markup language for GCL are here  [https://github.com/googlecodelabs/tools/tree/master/claat/parser/md](https://github.com/googlecodelabs/tools/tree/master/claat/parser/md)  but it is a basic guide.

Firstly we have to inform users what the document is about:

> author: Mariusz Saramak
> summary: TomTom Creating a custom Gangnam vector map style
> id: 24242443
> categories: sdk
> environments: js
> status: draft
> feedback link: github.com/tomtom-gangdam-style-for-map
> analytics account: 0

To specify the title of tutorial just use one “#” like below:

> # TomTom Creating a custom Gangnam vector map style

To specify the title of the first step, use two chars “##” right after title provide information about how much time user should spend on that part.

> ## Overview of the tutorial
> Duration: 0:05

#### Text and lists

Now we can add text, markup md language is simple. More information about md language you can find here  [https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

First text with lists:

> This tutorial shows you how to create custom vector map style. In this tutorial you will do the following:

> * Modify a default TomTom style for vector maps with use of the Maputnik editor
> * Apply the newly created style

> Prerequesites

> * API key
> * Npm and Node.js

> We recommend you to have npm and Node.js already installed on your machine to quickly boot up a http server.

until this moment we have that

[**Overview - first step · tomtom-gangdam-style-for-map/tomtom-gangdam-style-for-map.github.io@3da513b**
_Contribute to tomtom-gangdam-style-for-map.github.io development by creating an account on GitHub._github.com](https://github.com/tomtom-gangdam-style-for-map/tomtom-gangdam-style-for-map.github.io/commit/3da513b18c5d5e872e3001b56a9a51a73de7833a#diff-a7c1e55fe06fb49132a3116fdd55b78c "https://github.com/tomtom-gangdam-style-for-map/tomtom-gangdam-style-for-map.github.io/commit/3da513b18c5d5e872e3001b56a9a51a73de7833a#diff-a7c1e55fe06fb49132a3116fdd55b78c")[](https://github.com/tomtom-gangdam-style-for-map/tomtom-gangdam-style-for-map.github.io/commit/3da513b18c5d5e872e3001b56a9a51a73de7833a#diff-a7c1e55fe06fb49132a3116fdd55b78c)

Next we add some positive information:

> Positive
> : It is possible to have a single key(app) for all TomTom services, but you can also choose : to have individual keys for the different services.

We can add negative information too:

> Negative
> : To get an API key you need register or sign in to TomTom Developer Portal. Request an evaluation API key to access the service you want to use the SDK with.

Lets check what we have:

> //to convert md file to html file
> claat-linux-amd64 export gangnam.md

> //to download dependencies of html file and run a simple server on  [http://localhost:9090/](http://localhost:9090/#0)
> claat-linux-amd64 serve gangnam.md

#### Second slide and download link

> ## Download our Maps SDK offline examples
> Duration: 0:10

> Before you start, you need to download the latest version of our offline functional examples from [here]([https://developer.tomtom.com/maps-sdk/maps-sdk-downloads](https://developer.tomtom.com/maps-sdk/maps-sdk-downloads)).

But when we change “here” description to “Download functional examples” link for download will change to big green button.

#### Adding image



#### Adding code

> ``` bash
> npm install && npm start
> ```

Here we have example of adding bash snippet of code, but it can be any language. In example: java, kotlin, xml, js

We continue with tutorial and we should create document like that:

[https://raw.githubusercontent.com/tomtom-gangdam-style-for-map/tomtom-gangdam-style-for-map.github.io/master/gangdam.md](https://raw.githubusercontent.com/tomtom-gangdam-style-for-map/tomtom-gangdam-style-for-map.github.io/master/gangdam.md)

### What DOESN’T work

-   Force a new line. Md says about “\” two spaces, two enters, &nbsp; chars or <br/> I tried all and I can not force GCL to create new line :(
-   list with more then one level — I tried with no success.

> * list first level
> * list second level

-   list with URLs — When I tried to add URL to the link list, it didn’t generate a list
-   Download button — just doesn’t work

## Publishing a result

> ``` bash
> claat export doc.md
> claat serve doc.md
> ```


> Positive
> : It is possible to have a single key(app) for all TomTom services, but you can also choose : to have individual keys for the different services.

We can add negative information too:

> Negative
> : To get an API key you need register or sign in to TomTom Developer Portal. Request an evaluation API key to access the service you want to use the SDK with.

