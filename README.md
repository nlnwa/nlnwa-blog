# nlnwa-blog

To add content to nlnwa.github.io:

- New post:  
	```
	$ hugo new posts/loke.md
	/nlnwa-blog/content/posts/loke.md created
	vim content/posts/loke.md
	```

Start hugo server (with drafts) to see result:  
	```
	hugo server -D 
	```
Commit changes to repo:  
	```
	git add content/posts/loke.md
	git commit -m "Initial loke-post"
	git push
	```

To deploy/publish to blog:  
	```
	./deploy "New posts"
	```
(nothing is deployed because post is still draft)  

- Change draft to false  
- Push to repo:  
	```
	git add content/posts/loke.md
	git commit -m "Loke no longer in draft"
	git push
	```	

Deploy  
	```
	./deploy "Loke no longer in draft"
	```


# Static content (images)  
Static content is served from static/  
To add an image to a post:  
	```
	![Example](/path-in-static/image.png
	```
