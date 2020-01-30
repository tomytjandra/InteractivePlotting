# Interactive Plotting Quiz
___

In this quiz, we will be using a Youtube dataset (youtube.csv) and sample.html. You can get the file stored within the folder. The data has 2986 observations with 9 variables.


Here the list of the column variables :

 * `trending_date`: Video trending date
 * `title`: Title of video
 * `channel_title`: Name of the Youtube channel
 * `category_id`: Category of video
 * `publish_time`: Date the video was published
 * `views`: Number of video views
 * `likes`: Number of video likes
 * `dislikes`: Number of video dislikes
 * `comment_count`: Number of video comment

As a music enthusiast, you want to know 10 Youtube channels with the highest likes ratio.

```
 youtube %>% 
   ___(category_id == "Music") %>% 
   group_by(channel_title) %>% 
   ___(likes_ratio = mean(likes/views)) %>% 
   ___(desc(like_ratio)) %>% 
   ___(10)
```

1. Try to complete above code to get 10 YouTube channels with the highest likes ratio
  - [ ] filter, summarise,arrange,head
  - [ ] select, pivot, order, tail
  - [ ] filter, mutate, order, head
  - [ ] select, summarise, arrange, head

2. Based on `sample.html`, which one is the correct flexdashboard layout?
  - [ ] orientation: rows ; vertical_layout: fill
  - [ ] orientation: columns ; vertical_layout: fill
  - [ ] orientation: columns ; vertical_layout: scroll
  - [ ] orientation: rows ; vertical_layout: scroll

3. Which one from input type below is appropriate for categorical variable?
  - [ ] selectInput()
  - [ ] sliderInput()
  - [ ] plotlyOutput()
  - [ ] plotOutput()
  
4. Which of the following code is correctly paired between render and output in order to create plotly on shiny?
  - [ ] output$plot1 <- renderPlot({}) ; plotlyOutput("plot1")
  - [ ] output$plotly1 <- renderPlotly({}) ; plotlyOutput("plot1")
  - [ ] output$plot1 <- renderPlot({}) ; plotOutput("plot1")
  - [ ] output$plot1 <- renderPlotly({}) ; plotlyOutput("plot1")
 
