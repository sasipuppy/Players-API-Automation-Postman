# Players-API-Automation-Postman
Automating Player APIs using postman chai JavaScript tests. Stockholms Tekniska Institut Project

1.Postman tool--> PlayersAPI Collection --> Add requests
2.Set up environment, Add tests(javascript)-Chai is a BDD / TDD assertion library, set up workflow.
3.Execute the collection in collection runner
4.Export the environment and collections
5.Add the json files to the git repository
6. cmd cd C:\Program Files\Jenkins
7. java -jar jenkins.war --httpPort=8089
8. java -Dfile.encoding=UTF-8 -jar jenkins.war --httpPort=8089 (to fix html report issue)
9. http://localhost:8089
10. jenkins--> Freestyle project--> scm git (Add credentials for private projects, not needed for public)
   https://github.com/sasipuppy/Players-API-Automation-Postman.git
11. build-->Execute windows batch command 
12. newman run PlayersAPI.postman_collection.json -e PlayerEnvironment.postman_environment.json -r htmlextra
13. Generated Report: file:///C:/jenkins/workspace/PlayerAPI/newman/PlayersAPI-2021-03-16-08-35-52-201-0.html
