---
title: "Third Blog Post"
author: "Spencer Williams"
date: "2023-06-29"
---

I have found the Shiny R App creation and different methods for updating the UI are the most interesting to me. In other classes, I have seen professors use these shiny apps to produce different graphs from different distributions or samples. I had no idea that these were produced in R and that I can produce these now.

The conditionalPanel() method is unique to me in that I can change change plots or tables depending on the user checking a box within the app. Before this section, I would have had no idea where to begin in trying to create this operation.

For example, on the most recent homework, I used this line of code in the server.R file:

```
if(input$conservation){
      if (input$rem) {
        g + geom_point(size = input$size, aes(col = conservation, alpha = sleep_rem))
      } else {
        g + geom_point(size = input$size, aes(col = conservation))
      }
    } else {
      if (input$rem) {
        g + geom_point(aes(alpha = sleep_rem), size = input$size)
      } else {
        g + geom_point(size = input$size)
      }
```





