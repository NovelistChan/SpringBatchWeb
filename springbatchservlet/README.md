# SpringBatchSevlet
### version 1 (add mywriter)
 - Modified SpringBatch in demos to provide txt form outputs
 - 修改处：
   - 自定义Writer类：MyWriter，实现txt文本格式输出(调用Report中添加的toMyString()方法)
   - job-hello-world.xml(line 18、60): 添加step2(使用MyWriter进行输出，并做好了相应配置)
### version 2 (add servlet)
 - Add web.xml to springbatch
 - 修改处：
   - 添加package：servlet，内含Class：SimpleServlet实现web端操作
   - 添加配置文件webapp等，修改pom.xml
   - 最终实现效果为在localhost:8080/hello操作下，进行csv->txt的文件转换操作，并在web端输出提示文字
