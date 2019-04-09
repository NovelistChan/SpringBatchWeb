# SpringBatchMVC
### version 1 (add mywriter)
 - Modified SpringBatch in demos to provide txt form outputs
 - 修改处：
   - 自定义Writer类：MyWriter，实现txt文本格式输出(调用Report中添加的toMyString()方法)
   - job-hello-world.xml(line 18、60): 添加step2(使用MyWriter进行输出，并做好了相应配置)
### version 2 (add mvc)
 - add mvc framework to springbatch
 - 修改处：
   - 添加package：mvc，内含mvc框架实现Class：HelloController，在方法hello中添加对转换文本方法的调用
   - 添加配置文件webapp等，修改pom.xml
   - 最终实现结果为在原本MVC效果的基础上，会进行文本转换操作并在web页面中换行输出提示信息
