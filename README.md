# Module Graph Assert
This fork applies [this changes](https://github.com/jraska/modules-graph-assert/pull/176/files) to print out graph stats per module.<br>

Example output:

```
❯ ./gradlew generateModulesGraphNodeStatistics
Calculating task graph as no configuration cache is available for tasks: generateModulesGraphNodeStatistics
Type-safe project accessors is an incubating feature.

> Task :generateModulesGraphNodeStatistics
 node                   betweennessCentrality  degree  inDegree  outDegree  height 
 :core:data             72.00                  19      12        7          2      
 :core:datastore        16.50                  6       3         3          1      
 :core:testing          14.50                  10      3         7          4      
 :core:domain           14.00                  10      8         2          3      
 :core:ui               10.14                  12      8         4          4      
 :sync:work             3.00                   7       2         5          3      
 :feature:interests     0.14                   9       2         7          5      
 :feature:foryou        0.14                   9       2         7          5      
 :feature:bookmarks     0.14                   9       2         7          5      
 :feature:topic         0.14                   8       1         7          5      
 :feature:search        0.14                   11      1         10         6      
 :feature:settings      0.14                   8       1         7          5      
 :app                   0.00                   13      0         13         7      
 :core:common           0.00                   15      15        0          0      
 :core:designsystem     0.00                   10      10        0          0      
 :core:model            0.00                   16      16        0          0      
 :core:analytics        0.00                   11      11        0          0      
 :core:database         0.00                   2       1         1          1      
 :core:network          0.00                   3       1         2          1      
 :core:notifications    0.00                   4       2         2          1      
 :app-nia-catalog       0.00                   2       0         2          5      
 :core:datastore-proto  0.00                   1       1         0          0      
 :core:data-test        0.00                   3       0         3          5      
 :core:datastore-test   0.00                   3       0         3          5      
 :sync:sync-test        0.00                   3       0         3          5      

BUILD SUCCESSFUL in 3s

```
