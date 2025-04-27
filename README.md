> ggplot(combined_data, aes(x = Life, y = Death, color = group)) +
+     geom_point() +
+     facet_wrap(~ group) +  
+     labs(title = "Life Expectancy vs Death Rate Over Time",
+          x = "Life Expectancy (Years)", 
+          y = "Death Rate (Age-adjusted)",
+          color = "Sex") +
+     theme_minimal()                                        
> library(ggplot2)
> 
> ggplot(combined_data, aes(x = Life, y = Death, color = group)) +
+     geom_point() +  # Scatter plot for both men and women
+     geom_line(aes(group = 1), color = "gray", size = 0.5) +  
+     facet_wrap(~ group) +  # Facet by group (Men and Women)
+     labs(title = "Life Expectancy vs Death Rate Over Time",
+          x = "Life Expectancy (Years)", 
+          y = "Death Rate (Age-adjusted)",
+          color = "Sex") +
+     theme_minimal() 
