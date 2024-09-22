---
title: 
tags: 
date: 2024-09-22
toc: true
toc_sticky: true
---



# shrink git repo for obsidian android phone usage - wipback



## current state

![](../_asset/2024-09-22-git-blog-repo-shrink_image_1.png)

## Analysis Files and Sites 

![](../_asset/2024-09-22-git-blog-repo-shrink_image_2.png)

## Analysis Result

~ 50 % .pack Files 
~ 30 % PNG - Files 
~ 12 % JPG Files 

## Shrink .pack ?

https://stackoverflow.com/questions/11050265/remove-large-pack-file-created-by-git
https://www.ducea.com/2012/02/07/howto-completely-remove-a-file-from-git-history/
```
git verify-pack -v .git/objects/pack/*.idx | sort -k 3 -n | tail -5
``` 


![](../_asset/2024-09-22-git-blog-repo-shrink_image_3.png)

![](../_asset/2024-09-22-git-blog-repo-shrink_image_4.png)

## PNG - Shirinking in JPG /  WEBP
TODO -> PNG -> JPG / Webp + rename all Links 



jpg irfanview default, 80% quality


![](../_asset/2024-09-22-git-blog-repo-shrink_image_5.png)

Beispiel 2

![](../_asset/2024-09-22-git-blog-repo-shrink_image_6.png)


### Problem Webp 
![](../_asset/2024-09-22-git-blog-repo-shrink_image_7.png)

#### Finde relevant Files



## check Webp in Obsidian + git yekyll SSG Page - okay working 


![](../_asset/2024-09-22-git-blog-repo-shrink_image_8.webp)


## Results

- keine Dateien > 16383 Pixel Dim X or Y  für webp
- size webp < jpg 
- import as jpg / auto update PNG  
	- https://github.com/musug/obsidian-paste-png-to-jpeg 
	- https://gist.github.com/juanbretti/7f3dfc98b39e3d4216c275232a56305c