codium
======
An alternativ way to code your website.
A way to code more easily and with a good flexibility.

This is just a concept so currently no software can compile this language.
To be clear, in this concept we suppose that a browser is smart enough to understand this code. That's it that's all.



Forget about `<p>` `<i>` `<a>` `<e>` `<b>` `<div>` `<article>` `<main>` `<header>` `<ul>` `<li>` ....

Here, you can custom yours elements like you wish:

    [ menu ]  
        [ menu-list ]  
            Lorem 01  
        [/ menu-list ]  
        [ menu-list ]  
            Lorem 02  
        [/ menu-list ]  
    [/ menu ]  

Every element is a [ block ]
And here a way to give them some goodies:
     
    [ top | class='dark' | data='$valeur' ]
    
    [/ top ]
    
Yeah you can pass some variable if you need.

Another exemple:

    [ pub | src='img/pub.png'| href='pub.html' | alt='For Free Pub' /]

A block can be a link, an image or BOTH!

Different ways = more flexibility:

    [ p | text='Lorem ipsum dolor sit iaculis neque mollis in.' /]
or   
     
     [ p ] Lorem ipsum dolor sit iaculis neque mollis in. [/ p ]


Oh! And you can forget about `<doctypte>` `<head>` `<body>` `<html>` 
what you need to do is:

    [ head
	    | charset='utf-8'
	    | title='bonjour'
	    | src='../css/main.css'
    /]

or if you want:

    // head
    [ charset='utf-8' | title='bonjour'	| src='../css/main.css' /]

and in the bottom of your site:

    //foot
    [
        | src='../js/plugins.js'
        | src='../js/script.js'
    /]

Last exemple:

    [ table | class='fancy' ]
        [ table-row ]
            [ table-col ]
                01
            [/ table-col ]
            [ table-col | class='win']
                02
            [/ table-col ]
            [ table-col ]
                03
            [/ table-col ]
        [/ table-row ]
    [/ table ]


And about the semantic?
Well I suppose that each element can be define in an other file in jSon:

    { 
        "content": {
            "role": "main",
            "type": "list",
            "rel": "me"
        }
    }

Not sure about this part... need time to think about it



    


