---
title       : Reservoirs
subtitle    : 
author      : Developing Data Products course project
job         : January 2015
framework   : io2012       # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---
<style>
.title-slide {background-color: #0f5feF}

.title-slide hgroup h1 {
  font-size: 65px;
  line-height: 1.4;
  letter-spacing: -3px;
  color: #FFFFFF;
}



.title-slide hgroup h2 {
  font-size: 34px;
  color: #FFFFFFF;
  font-weight: inherit;
}




</style>



## Everything's bigger in Texas
###  including drought & flood 

<!--- 2-column example from http://rmarkdown.rstudio.com/ioslides_presentation_format.html --->

 <div class="columns-2">

<br>
  
 The state of Texas (USA) spans a large geographical area, with severe drought in western regions coinciding with a rainy season in the east.

<br> 

This figure shows the recent status of water reservoirs statewide as a percentage of filled capacity. 
<br> [Image credit:  Texas Water Development Board, waterdatafortexas.org]

 
 <img src="recent_conditions.png" width="500">  
 
 
</div>


For the course project, I developed a shiny application that illustrates changes in reservoir water levels through time. The app loads datasets for individual reservoirs  and calculates summary statistics for a selected year, and plots the highlighted year along with the historical record. 
<br>
 
 


---  .class #id

## Shiny app screenshot


<img src="reservoir_screenshot.png">


---  .class #id


## Reservoir Stats






```r
# Example calculations for summary statistics during selected year.
mean(reservoir_selected_year$percent_full)  
```

```
## [1] 54.33361
```

```r
min(reservoir_selected_year$percent_full)
```

```
## [1] 34.5
```

```r
max(reservoir_selected_year$percent_full)
```

```
## [1] 79.3
```

```r
# Note: calculations valid when storage capacity is constant throughout selected year [generally true]
```

---  .class #id


## Acknowlegements
 
 <li> Texas Water Development Board (TWDB), waterdatafortexas.org  </li>
 <li> Developing Data Products discussion forums </li>
 <li> stackoverflow.com </li>
 
 
 
 



