# Managing Multiple Pages


There are currently two strategies for structuring multiple pages in one repository.


## Simple flat project with no hierarchy of pages

If your documents are going to consist of just a few pages, the simplest way to get started is just by placing all of your .md files in the root directory of your repository.  All files can link to each other directly without having to worry about paths.  For example README.md can link to file-a.md with \[File A](file-a.md).   file-b.md can links to file-a.md with \[File A](file-a.md).  File B can link to README.md with \[README.md](README.md). 

This strategy has the added benefit of working well on http://prose.io because you can create new files in a repository but you cannot create new folders.  However, your links will not path correctly when previewing them on Prose.io. 

As for images, you can place an image in the root directory and path the images as you would path to a page, or if you have a lot of images it can be "more elegant" to place them in an images directory and path them like \![Cool image](images/cool-image.png).  


## Complex project with a hierarchy of pages

Building on GitHub's subtle yet powerful README feature, you can create a hierarchy of posts using folders with the text for each folder saved as a README.md file in that folder's directory. If you are familiar with the behavior of index.html on web servers, you will feel right at home with this technique.  In this case, File A would not live in the root directory as file-a.md but instead lives in a folder named file-a with a text document README.md (file-a/README.md).  To link to File A from the root README.md file you would path a link like \[File A](file-a) which would then forward the user to the folder folder-a with GitHub displaying the current file-a/README.md file on the page.

This technique also has the advantage of keeping the images of each document close to the text of each document.  Do this by placing the images for each folder's README.md in the same folder as its corresponding README.md file. 

