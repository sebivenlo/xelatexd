# xelatexd
xelatex docker image with utility scripts to work as like gradlew or mavenw



## Installation

1. Clone this directory.
2. Change into the directory of this clone.
3. Build the docker image with `docker build -t xelatexd .` This may take some time, because it pulls in a linux plus full texlive installation into the image.
 You need to do this only once, and it will take less time on a fast connection.

## Use

1. Copy the **docker-compose.yml-example** to your (xe)latex document's root folder. Name the docker-compose file **docker-compose.yml**
2. Copy the file latexw to the root folder of your project. Same for the file bibtexw (they are the same, in a *NIX installation they can use a sym link.)
2. Start container from the created image with `docker-compose up -d`. You need to do this only once in a session.
3. Use the wrapper script (which needs bash) **./latexw** for your latex runs and bibtexw for your bibtex run.

enjoy.
