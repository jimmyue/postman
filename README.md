#https://www.jianshu.com/p/b1771113162d


#postman导出接口和环境变量，根据环境变量执行json接口

newman run collection.json -e environment.json -g globals.json


#执行json接口，生成报告

newman run collection.json -e environment.json -g globals.json -r htmlextra --reporter-html-export htmlReport.html
