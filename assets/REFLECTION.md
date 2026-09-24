Describe the path an HTTP Request takes from a browser to your GitHub Pages site.

Answer: If i were to input my github repository link into the browser, it essentially uses a domain name sys (DNS) to look up the IP address of GitHub's servers. It's equivalent to looking up a word in a dictionary. The browser would open a connection to the server using TCP and ensures that data will arrive in completeness and also in correct order. Since the site uses HTTPS, the browser and server sets up a TLS which helps encrypt connections and confirms the server "owner." With the secure connection created, the browser sends a HTTP request for the page and then GitHub finds index.html in my repos to send it back with a 200 OK response. Then it reads the browser html and then sends another request for css file and then it compiles on screen. 

AI Attribution
I used Claude to help with the CSS style of the portion.
Prompts I used: 
Why did my #name not win even though its an ID selector from my code:
    h1 {
        color: red;  
    .title {
        color: purple;
    }
    #name {
        color: navy;
    }
Logic error I fixed: My h1 rule was missing a closing }, so the
browser ignored my .title and #name rules and my name stayed red. It was a small typo and didn't look close enough. 