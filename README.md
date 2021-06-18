# coming-soon
Simple customizable web page to signal the imminent implementation of a project. The page is provided with a Docker container.

----
## Requires 

### Docker

See [Docker](https://www.docker.com/) and [Docker-compose](https://docs.docker.com/compose/)

### Sass

See [Sass](https://sass-lang.com/install)

----
## Usage
1. Run docker-compose 
```docker-compose up -d```
2. Open the address localhost:91 on your browser

----
## Change CSS
```cd scss && sass --watch soon.scss:../html/dist/css/soon.min.css --style compressed```

The images are in the file "scss/components/_carousel.scss".

----
## Countdown

Simply change the "deadline" variable in "html/index.html".

To switch to French day ("j" instead of "d"), set the "isDayFrench" variable to true.

```
  // Countdown configuration
  var current_date = new Date();
  var year=current_date.getFullYear();
  var year=year+1;
  var deadline="Jan 1, "+ year +" 00:00:00";
  var isDayFrench = false;
```