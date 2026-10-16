hw 1:

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

hw 2 additions:

Explain the difference between flex-direction: row and flex-direction: column.

Answer: The difference is that flex-direction sets the way items in a flex container line up and flex:direction: row is when items sit side by side from left to right, this is the default. flex-directions: column stacks the items top to bottom like a list (1,2,3...) where 1 is the top and 3 is the bottom.

Why is it important to use relative units (like %, vh, or rem) instead of fixed pixels (px) for
responsive design?

Answer: Its because fixed pixels will always be the same size, an example would be that I cannot fit a large pixeled image from a laptop to a phone. So if I were to display it on the phone, you would essentially have to scroll around to see the full image. % allows us to scale with the parent element, vh and vw will scale to the screen and rem scales with browser's font size. For example, the project cards in my code use a width: 50% so they are half the width of the card. They will shrink automatically when grids collapse on the phone instead of staying a fixed size, which allows it to be functionally adaptable across browsers essentially.
