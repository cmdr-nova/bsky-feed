# bsky-feed
A simple piece of JavaScript that'll display your Bluesky posts on a website. All you have to do is edit the top content of in the JavaScript, and then add each piece to your website, and you're done.

Note: There is a proxy server function within the script, because I was having *major* issues with CORS errors, and the default solution was to just bounce off of some free solution. A solution that turned out to be restricted and a "demo." So, I setup a CORS proxy on my VPS with node and pm2 and directed all feed traffic through *that* proxy and it works.

If you **don't** have CORS issues, you can just completely remove the proxy function, and the script will move forward without it. But, I'm assuming you probably don't want to do that. For hosting a proxy I would recommend a cheap VPS. I have a 6 USD VPS at Digital Ocean that's running all of my Python scripts, and also a constant proxy server that I bounce some of my website's content off of. It's fast, easy, and there are no headaches with CORS.

Heckin' CORS, man.
